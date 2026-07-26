# Basic Employee Onboarding (AD)(RBAC)

## Problem Statement
* The problem in this project was related to a fictional company called Northstar Medical Group. They started off as a smaller company and were using an MSP to manage their Identity Lifecycle workflows as they didn't have the means to manage it themselves. Initially it worked fine, but as the company grew they started to notice issues that could not be allowed to continue. Users either had too much access or not enough, there were NO RBAC policies in place leading to audit and HIPPAA risks. There was no organization and when employees left the company sometimes it would be months before their accounts were disabled. As for new hires, sometimes it would take days to get them the proper access as nobody documented or knew the process to do so.

## Solution Overview
* The solution was to build out a basic employee onboarding process in Active Directory. I set up RBAC to ensure users only got access to the systems and information required for their roles. To simulate one such issue, I created a mock ticket where a user was provisioned with the incorrect level of access. I started by creating the domain from scratch by adding the Active Directory Domain Services role to the server and promoting it to a domain controller. I then added the OUs to organize the domain by department, after which I added the security groups for each OU so when I added the users through PowerShell I could ensure they were added to the appropriate security groups ensuring they were provisioned properly.

## Video Walkthrough
https://github.com/user-attachments/assets/c5951330-54c1-40c9-91a4-2bd1f7d4c97f

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub
* PowerShell

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Solved a mock ticket where a user was given incorrect access
* I fully documented my steps end-to-end
