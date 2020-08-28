# Ops Challenge: Sendmail

## Overview

In 1979, Eric Allman wrote the original ARPANET delivermail, one of the earliest forms of email ever developed. Allman went on to write Sendmail in the early 80s at UC Berkeley. Sendmail shipped with BSD in 1983. By 1996, 80% of internet mail servers used Sendmail to deliver email. The ability to send email from a Linux server is useful for notifying administrators of events taking place on the server. In today's Ops Challenge, you will be installing Sendmail on your Ubuntu Linux VM and using it to send emails via SMTP protocol.  

## Resources

- Ubuntu Linux 20.04 Focal Fossa VM from [osboxes.org](https://www.osboxes.org/ubuntu/)
- Gmail account

## Feature Tasks and Requirements

Firstly, created a dedicated Gmail account to use for this exercise. Toggle ["Allow less secure apps"](https://myaccount.google.com/lesssecureapps) to ON to allow Sendmail SMTP access to your Gmail.

Now, access your Ubuntu VM. 

- Install Sendmail. In terminal, run `apt-get install sendmail mailutils sendmail-bin`
- Create a new directory called authinfo in your etc system folders. `mkdir -m 777 /etc/mail/authinfo/`
- Go there. `cd /etc/mail/authinfo/`
- Create a file called gmail-auth. Open the file with a text editor and enter `AuthInfo: "U:YOUR UBUNTU USERNAME" "I:YOUR GMAIL EMAIL ADDRESS" "P:YOUR PASSWORD"`
- In that folder, make a hash map for the gmail-auth file. Run `# makemap hash gmail-auth < gmail-auth`
- In /etc/mail/sendmail.mc find the first "MAILER" definition line and paste the below right above it:
```
define(`SMART_HOST',`[smtp.gmail.com]')dnl
define(`RELAY_MAILER_ARGS', `TCP $h 587')dnl
define(`ESMTP_MAILER_ARGS', `TCP $h 587')dnl
define(`confAUTH_OPTIONS', `A p')dnl
TRUST_AUTH_MECH(`EXTERNAL DIGEST-MD5 CRAM-MD5 LOGIN PLAIN')dnl
define(`confAUTH_MECHANISMS', `EXTERNAL GSSAPI DIGEST-MD5 CRAM-MD5 LOGIN PLAIN')dnl
FEATURE(`authinfo',`hash -o /etc/mail/authinfo/gmail-auth.db')dnl
```
- Rebuild sendmail's configuration. Run `# make -C /etc/mail`
- Reload the Sendmail service with `/etc/init.d/sendmail reload`

Sendmail should now be ready for use.

- Send an email from terminal using `$ echo "Just testing my sendmail gmail relay" | mail -s "Sendmail gmail Relay" [DESTINATION EMAIL ADDRESS]`

Explain in your own words why sending email from a server could be a useful capability for a systems administrator. How might this capability be abused for malicious intent? Name the type of attack this kind of automation would facilitate and define it.

Include in your submission a screenshot of your successful email terminal command and your recipient inbox showing the email arriving.

## Stretch Goals (Optional Objectives)

Pursue stretch goals if you are an advanced user or have remaining lab time.

- Configure a bash script you already wrote in a previous Ops Challenge to send an email to you describing the results or listing the output of the bash script.

## Submission Instructions

- When you are ready to submit your shell script for grading, copy your script to a new file in your **public** [Github](https://github.com/){:target="_blank"} repository. Name the file according to your cose code and assignment, e.g. `ops-301d1: Challenge 01`.
- Copy the URL to your Github file and paste below as your submission. Add a comment in your Canvas assignment which includes the following:
    - A question within the context of today's lab assignment
    - An observation about the lab assignment, or related 'Ah-hah!' moment
    - How long you spent working on this assignment




