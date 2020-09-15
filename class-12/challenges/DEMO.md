# Ops Challenge - Psutil 

## Demo Code

The demo code below introduces concepts necessary to complete the challenge. 

```python

# Installation: https://github.com/giampaolo/psutil/blob/master/INSTALL.rst

# Docs: https://psutil.readthedocs.io/en/latest/

# Libraries are imported at the top of any Python script using syntax import [library]

import psutil

# Generate CPU times as a named tuple

print(psutil.cpu_times())

# Show current CPU consumption wrapped in explanatory text

print("Current CPU consumption is",psutil.cpu_percent(),"percent.")

# Show physical cores wrapped in explanatory text

print("I have",psutil.cpu_count(logical=False),"cores in this CPU.")

```


