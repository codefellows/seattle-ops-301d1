# Ops 301 Final Project Guidelines

## Conflict Plan

Your team should agree on a process for handing disagreements, should they arise. It is better to have a plan in place ahead of time so you can all refer back to it if necessary.

_Why:_
> Project week can be stressful and emotions can run high. Put together a plan ahead of time so you all know how to deal with any potential issues later.

As a team, create a Group Agreement as a markdown file to document the following:

* What will your group do when it encounters conflict?
* How will you raise concerns to members who are not adequately contributing?
* What is your process to resolve conflicts?
* How and when will you escalate the conflict if your attempts are unsuccessful?

## Communication Plan

Before beginning to tackle the project, determine how your group will communicate with each other. 

_Why:_
> This is not an individual effort. Make sure everyone knows how the group will communicate with each other and that everyone feels comfortable speaking up.

Add your communication plan to your Group Agreement. Some things to consider:

* How will you communicate after hours and on the weekend?
* What is your strategy for ensuring everyone's voices are heard?
* How will you ensure that you are creating a safe environment where everyone feels comfortable speaking up?

## Project Scope

Determine which features make up your minimum viable product (MVP). This should include any features you absolutely want to have in your application for presentation day.

_Why:_
> Scope creep can be dangerous! Keeping your project within a pre-determined scope will help the group stay on task without going off on tangents and side features.

Beyond MVP, put together a list of stretch goals to tackle if you have time. During your pitch, your instructor will help you scope your project. Some features may become MVP and some may become stretch goals.

Once you are ready, find your instructor and pitch your idea.

## Daily Team Workflow

As a team, decide how you will work on your project throughout each day.

_Why:_
> Ensure that everyone is on the same page about the current status of the project and the plan for the day.

At the beginning of your day, it is helpful to have a meeting between the team members to make sure that everyone knows what is going on with the project and to discuss the plan for the day. It is wise to have additional check-ins partway through the day and at the end of the day. With every check-in, assess the current percentage of MVP and make a prediction for when your team will reach full MVP.

During your team check-ins, discuss the features each member plans to work on. Determine if the team member will work individually, as a pair, or if the entire team will work on a single feature together, referred to as "mob programming".

Also, use this time to discuss any interpersonal issues that may arise. It is better to address them head-on and resolve any tension rather than allowing it to fester.

## Standup

Every day, the instructional team with circulate to your group for a formal "Standup Meeting". Standup should take approximately 10 minutes per team. Some instructors will opt for a second standup later in the day.

_Why:_
> Standups give the instructional team insight into the current status of your project and the progress the team hopes to make each day.

During standup, each team member will stand up and take turns discussing three points:
> 1. What you personally accomplished yesterday
> 1. What you plan to accomplish today
> 1. Anything that is blocking you from making progress

## Presentation Prep

Your team should practice your presentation prior to the final presentation day. This is typically scheduled by the instructional team. During the practice presentation, the instructional team will provide constructive feedback about the flow of the presentation and appearance of the application.

_Why:_
> If there are any issues in your final product's functionality or appearance, it is better to catch them ahead of time. This is also an opportunity to view the application as it will be shared with the audience. Evaluate any screen size issues, color changes due if you are projecting, and overall impact on the user's experience. The practice round will also allow the team to work on the flow of the presentation as speaking roles are passed from one member to another.

Decide whose computer to use during the presentation and have that computer fully ready for practice session. Make sure you have any cables or adaptors needed, and know what settings are needed to share your screen (and audio, if relevant). Test this computer as the driver of the presentation BEFORE your practice. Test a backup computer as well, just in case.

The presentation should follow exactly from the [template slide deck](https://docs.google.com/presentation/d/1ObrNpOqGhyaKRTIDXnFaIRVKMBGiiCiFkfJJ9T2xi_s/edit#slide=id.g8526846ab1_1_35){:target="_blank"}. Ensure your timing is no more than 15 minutes long, including some time at the end for questions. Present from the final product, deployed site, or offical documentation that you produce. Each member should introduce themselves with their personal pitch. The "About Us" page provides a great backdrop for this portion of the presentation.

Each member of the team must have a speaking part. It is okay to use note cards if you are nervous about forgetting what to talk about. Some of the areas to discuss include:

- An introduction of the project and the problem domain, including the team's solution
- A demonstration of the final product: highlight your organization, functionality, and all deliverables from the requirements
- The team's approach to planning and communication throughout the project
- A technical obstacle or two and how those obstacles were overcome
- A portion of the final application that each team member is particularly proud of

In general, do not show code during the presentation unless the audience asks to see it. Have a code editor open just in case though.

The appropriate dress code is business casual - not too formal and not too casual.

In addition to the scheduled practice session, the team is encouraged to continue to practice on their own. Keep track of the time and adjust accordingly. Practice with the microphone (muting / unmuting, or holding something if in-person) to feel comfortable with it, and practice passing the microphone between team members as you switch speaking roles if in-person.

Speak clearly and do not use slang or profanity. Take it seriously and be professional.

## Grading

Each team member's grade is split between their individual effort, and the project's technical merit.

Individual effort is graded based on contributions to project deliverables, and professionalism in the presentation.

Technical merit of the project overall is evaluated according the requirements. 

### Scenario

Your team is a cloud consulting firm specializing in cloud infrastructure and automation. You are currently in early stage talks with a [client company](https://www.builtinseattle.com/companies/best-midsize-places-to-work-seattle-2019) who has submitted a request for proposal (RFP) to migrate the company's existing on-prem infrastructure to the cloud. As part of the desired change, your client would also like to transition to a DevOps methodology when it comes to the deployment and upkeep of its new cloud infrastructure. The board of directors would like to see, in a single presentation, how this can be accomplished with your help. Your presentation should present a compelling case to work with you for this project.

- Choose a [client company](https://www.builtinseattle.com/companies/best-midsize-places-to-work-seattle-2019) as your example.  
  - Company size: Mid-sized (roughly 500 people but larger is acceptable to use)
  - Use only publically available information/intelligence about the company. Dig deep to see how much you can learn!
  - Do not fabricate information to fill in gaps.
  - Do not include sensitive or confidential information such as vulnerabilities identified during your research of the organization.
- Your proposal will be to the executives at the company.

### Presentation

Components of the presentation must include:

- Introduce your cloud consulting firm by name, and team members.
- As the "Problem Domain", describe the company you selected. Highlight what you researched about the company from public information, and why your company is a good fit (eg: why you selected this company for this project).
- Discuss the client engagement proposal.
- What will you do to transition the organization to a DevOps cloud infrastructure? 
  - Each student must create and submit one working script that automates cloud system deployment or an aspect of the migration to cloud
  - Cost analysis of both the process of migrating to cloud/DevOps style administration and monthly operational expenses (OpEx) associated with cloud usage.
- Use a network diagramming tool to create a network diagram of the organization’s cloud environment.
  - In GNS3 create a working LAN that depicts the company's remaining on-prem environment.
  - Depict in both how your network accomodates up to 25%-90% of your employees being remote work from home (WFH) employees.
  
- Present live technical demonstrations
  - All team members must present an equal share of the live technical demonstrations.
  - Live technical demonstration of the new cloud environment via IaaS provider's web administration portal:
    - Create a private cloud using one of the top IaaS providers (e.g. AWS, GCP, Azure, IBM Cloud, Oracle Cloud).
    - Demonstrate how encrypted connectivity to the private cloud is performed from a local host. 
    - Demonstrate how the deployment and configuration of a cloud server (one of the below components) can be achieved on this platform using infrastructure-as-code (IaC) scripting automation. 
    - Your team will select a script and demo it during the live presentation
    - Include in your cloud environment the following components:
      - AD/Domain Controller(s)
      - Web Server(s) 
      - File Server or cloud-based file sharing platform(s)
      - Endpoints
    - Include evidence that the above components will be deployed with security best practice configurations.

### Proposal Deliverable 

Submit to instructor a single proposal. The document must be submitted as a Google Doc, with a complete version history showing how it was created. All team members are to contribute an equal share to the proposal and should clearly indicate which components each contributed to in their individual project submission notes.

Here is a list of requirements the board of directors would like to see addressed in your proposal:
- Central administration of all Windows-based computers
  - A network topology diagram of your new cloud-based systems architecture design, pasted into your Google Doc.
  - All components must be labeled, and network diagram must be presentable (straight lines) and free of defects/typographical issues. Take your time to create a quality network diagram; do not rush!
- How the cloud environment's core network services will be administered
  - Explain and justify your network diagram in detail. Clearly indicate what devices are hosting network servers DHCP and DNS. 
  - Provide network configuration details.
    - DHCP range
    - Subnet mask
    - IP address of all devices clearly indicated on network diagram
- How will OS version control be handled?
  - Describe in detail how OS version control will be handled centrally from a server-based solution. Hint: Read [Windows Server Update Services](https://docs.microsoft.com/en-us/windows-server/administration/windows-server-update-services/get-started/windows-server-update-services-wsus){:target="_blank"}
- Physical hardware requirements of your proposal
  - List all specs (similar to scenario hardware specs list above) of your cloud machines
- Software requirements of your proposal, inluding all required licensing. Clearly indicate all software **versions** and **editions** to be used in your solution.
- All associated costs including sourcing information, including who will you purchase all this from, at what price, and what terms.
  - Include a projection of monthly overhead based on anticipated usage for given rates
  - REMEMBER: A lower-cost proposal is more likely to be approved. While a budget was not specified, this organization is cost-sensitive at this stage to technology infrastructure purchases.
- How will you migrate some on-prem systems to cloud DevOps style administration?
  - Include a realistic timeline of implementation including major milestones. Create a project plan using a project management software of your choosing and include screenshots in your Google Doc submission accompanied with explanatory text. Justify your choice of milestone dates and why you believe these to be realistic estimates.

Include in your proposal any changes that need to be made to endpoint systems specs and/or network infrastructure configuration, and why these changes are necessary.
While this is not an internal RFC, include in your proposal all required elements for an [ITIL-compliant Request for Change (RFC)](https://wiki.en.it-processmaps.com/index.php/Checklist_Request_for_Change_RFC){:target="_blank"}. Exclude the RFC number.

