# Morris-Worm-Digital-Forensics-Lab
By: Joshua Radjavitch and Jared Burns

Steps to replicate the Lab:
- Download and setup the SEED Ubuntu 20.04 Virtual Machine
- Unzip and import the Labsetup.zip folder found in this repo onto the VM
- Build and start either the mini internet or the nano internet using Docker
- Enter the command `sudo /sbin/sysctl -w kernel.randomize_va_space=0` in a terminal on the SEED machine to turn off memory randomization
- Open Firefox on the SEED machine and navigate to http://localhost:8080/map.html to view the map of the mock internet
- Run the worm.py script found in the worm folder to release the worm on the mock internet
- On the map, watch the worm spread throughout the internet
- Open a terminal on one of the infected machines
- Investigate using commands such as ps aux, stat, and ls bof to find out more about the Worm on both the SEED machine and the machine in the mock internet
- Assemble a timeline of events using the information you found in your investigation
