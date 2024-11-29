Hosting a Resume/Portfolio in EC2 instance with CI/CD setup using GitHub

Followed the below steps to achieve this,
  Created a EC2 instance in AWS Console with Ubuntu OS and Security group allowing Port 80, Port 443 from anywhere in internet
  Along side created a KeyPair for the EC2 to make it accessible to the GitHub deployment/changes
  Stored the secrets in the Github from the EC2
  Created a YAML file for the CD/CI setup and so whenever a deployment/changes happens it triggers the changes to be get published in the EC2 lying source code of the Resume/Portfolio
  
What we acheived
  We made the GitHub to access the EC2 instance to update the source code of the Resume/Portfolio in the server whenever a changes/Deployment happening in the GitHub.
  the YAML file will take the responsiblity to deploy the new changes in the Git to the EC2 by running a simple SSH commands on it
  

<!--
**Sunilkumaur/sunilkumaur** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
