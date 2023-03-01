# Module 5 Demo Project - Cloud and Infrastructure as a Service Basics

# Demo Project - Create server and deploy application on DigitalOcean

### Steps
1. Set up account on DigitalOcean
2. Create a droplet
3. set up ssh key to use for droplet login. Run `ssh-keygen` on local machine and copy public key to Digital Ocean 
4. Set up firewall rules (inbound on port 22 - ssh) and add droplet
5. ssh into droplet on local machine (assuming root)
6. run `apt update` to update instance
7. install java with `apt install openjdk-8-jre-headless`
8. Build java project locally
9. secure copy jar file from build to the digital ocean instance
10. run the jar file on the instance with `java -jar <jar_filename>`
11. The application will be running on port 7071. To access it from the public internet open the open 7071 inbound on the firewall.
12. create a new user `useradd <username>`
13. add the user to the sudo users groups `usermod -aG sudo <username>`
14. switch to user `su - <username>`
