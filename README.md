# HAZESOFT-T2

Step 1: 
Installing ansible 
Commands
- sudo apt install software-properties-common
- sudo add-apt-repository --yes --update ppa:ansible/ansible
- sudo apt install ansible

Step 2:
After the ansible is successfully installed my next step was to create the ansible playbook which can automate the following tasks
- install nginx
- install git
- clone git repo to temporary folder
- copy the site folder to nginx root folder
- copy custom configuration file in place nginx default configuration
- Restart the nginx service to accomodate the changes

Step 3:

Run the ansible playbook
- To run this ansible playbook first you need to have the configuration file in the same location as the playbook  
- By givig simple commands ansible -playbook task.yaml you can run and experience the changes in your localhost.
- Commands

------- ansible-playbook task.yaml



Varifying the task is compleated 
-- you should see 9 changes and you can symply run this command to verify the system is up and running
Command

----- http://localhost:9000/site/index




NOTE : to deploy this ansible playbook to other hosts linked with the master you can simply give hosts as "all" or the particular host's name.




------- For the configuration file
Step 1:
- I have changed the service to listen to port 9000 instead of default port 80
- I changed the root directory from /var/www/html/ to /usr/share/ngnix/html/



############################# THANK YOU !!!! ###############################
