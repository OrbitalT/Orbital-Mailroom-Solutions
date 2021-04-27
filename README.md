# Orbital-Mailroom-Solutions
This is a Mailroom Management tool was made out of necessity for my current job.

# Why
The problem, we get to many packages and we dont know how many each person has.

# Goals
Lable each package with its unit number and (QR code see below)
Add each new package to a database (SQL)
keep track of how many packages each unit has
Send email to inform of package
Remove package form DB with QR code

# Needs
This project will use:
- Raspberry pi 3
- pi cam v2
- Micro sd (8GB)
- Power (Micro USB)
- Keyboard
- Monitor
- Thermal Printer

# Approach
Input
1. Package comes in
2. User adds package to unit through CLI (Ex. 705 1) (GUI in V2)
3. System adds package to unit then prints a QR code with unit number on sticker (QR tells DB to remove 1 from that unit Check Out)
4. User adds sticker to package then stores on shelf
5. System will send email to units with and updated package total (HTML) (Can be configured to only send from direct User input) (System Backend V2)

Output
1. User asks system to show units packages (Ex. show 705)
2. System will print units packages (Ex. 705 => 2 Packages)
3. User will get packages and scan into system
4. System will remove each package from Units package total
