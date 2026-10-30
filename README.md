# User-Management-on-Linux-CLI
This is a mini project aimed to add and manage users with Linux commands
# Task Overview
First, I'll add a new employee to the system and then to their primary group. Second, I'll make this employee the owner of a file related to a particular project. Third, I’ll add the new employee to a supplementary group. Finally, I’ll delete the employee from the system.
# Add a new User to system
sudo useradd researcher9
# Add User to group research_team
sudo usermod -g research_team researcher9
#  Assign file ownership in /home/researcher2/projects/project_r.txt
sudo chown researcher9 /home/researcher2/projects/project_r.txt
# Add the user to a secondary group
sudo usermod -a -G sales_team researcher9
# Delete a user
sudo userdel researcher9
sudo groupdel researcher9
