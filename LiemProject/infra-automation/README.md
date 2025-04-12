# ⚙️ LiemProject – DevOps Provisioning Simulation Tool

## Overview

LiemProject is a DevOps simulation tool designed to:
-⁠  ⁠Collect user input to configure a virtual machine.
-⁠  ⁠Validate input using a JSON schema.
-⁠  ⁠Save configuration data to JSON.
-⁠  ⁠Simulate service provisioning Nginx installation using a bash script.

This project focuses on practicing infrastructure-as-code concepts and automation logic in a simplified, modular way.

## Objectives

- ✅  Dynamic user input for VM creation 
- ✅  Input validation using [JSON Schema]
- ✅  Configuration saved as JSON (`configs/instances.json`)
- ✅  Bash script simulates Nginx installation with feedback
- ✅  Logging to file: `logs/provisioning.log`
- ✅  Modular code with a `Machine` class

---

## Example Output
Enter VM name: server liem
Enter OS (Linux Ubuntu / Windows 10):  linux
Enter number of CPUs: 10
Enter amount of RAM (GB): 4

✅ Good input
{'name': 'server liem', 'os': 'linux', 'cpu': 10, 'ram': 4}
✅ JSON schema validation passed.

[✔] Checking if Nginx is installed...
[i] Nginx is not installed. Simulating installation...
[✔] sudo apt update
[✔] sudo apt install -y nginx
[✔] sudo systemctl start nginx
[✔] sudo systemctl enable nginx
[✔] sudo systemctl status nginx
[✔] Status: Nginx is running successfully

## Setup Instructions
- Check that all conditions from the Requirements file are present.
- You're ready to run the simulation

### Requirements

- Python 3.7 or higher  
- `jsonschema` module