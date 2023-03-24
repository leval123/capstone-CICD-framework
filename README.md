# Continuous Integration 🛠️ DevOps Pipeline 👨‍🔧
End-to-end DevOps testing framework for made using 🐍 Python, 👨🏻 Jenkins, 🐶 DataDog, 🪣 Git, and 🔎 Elastic Search! :scream::scream:

Includes a separate 🤖Android based infotainment system for a potential test bench. 
This project is basically a DevOps pipeline for developing applications and lets you run an integration build every time you push a change to your Git repository. 

### Configuring your GitHub repository

Step 1: Go to your GitHub repository and click on 'Settings'.

Step 2: Click on Webhooks and then click on ‘Add webhook’.

Step 3: In the ‘Payload URL’ field, paste your Jenkins environment URL. At the end of this URL add /github-webhook/. In the ‘Content type’ select: ‘application/json’ and leave the ‘Secret’ field empty.

Step 4: In the page ‘Which events would you like to trigger this webhook?’ choose ‘Let me select individual events.’ Then, check ‘Pull Requests’ and ‘Pushes’. At the end of this option, make sure that the ‘Active’ option is checked and click on ‘Add webhook’.

### Configuring Jenkins
Step 5: Download Jenkins (Generic Java package (.war)): https://jenkins.io/download/

Step 6: Execute Jenkins as a Java binary (java -jar ./jenkins.war)

Step 7: In Jenkins, click on ‘New Item’ to create a new project.

Step 8: Give your project a name, then choose ‘Pipeline’, name it whatever you'd like and finally, click on ‘OK’.

Step 9: Configure and execute pipline job through any script file in the repository as needed (feel free to test!) by choosing "Pipeline script" as Destination and pasting the contents into Script.

Step 10: Configure to modify the existing job, go to 'Advanced Project Options' and then click 'Pipeline script from SCM'. 

Step 11: Click on Git and paste your GitHub repository URL in the ‘Repository URL’ field.

Step 12: Click on the ‘Build Triggers’ tab and then on the ‘GitHub hook trigger for GITScm polling’. Or, choose the trigger of your choice.

![image](https://user-images.githubusercontent.com/53611087/198152478-88bdaeb9-c13f-4a48-835e-e8e0ace66159.png)

## Thank you for checking it out! :metal:&#127999;
