Hosting My Portfolio in AWS EC2 instance with CI/CD setup using GitHub

I hosted my resume and portfolio on an EC2 instance with a CI/CD setup using GitHub. 
To start, I created an EC2 instance on AWS running Ubuntu and configured the security group to allow HTTP (port 80) and HTTPS (port 443) access from anywhere, 
ensuring my portfolio is publicly accessible.
          
I then generated an SSH keypair, which allowed secure communication between GitHub and 
the EC2 instance for automated deployments whenever there were updates to the repository. To keep things secure, I stored sensitive data, 
like the SSH private key, in GitHub secrets, ensuring that no credentials were exposed.

Next, I set up a YAML file in the .github/workflows directory to automate the deployment process. 
This configuration allows changes pushed to the main branch of the GitHub repository to trigger a deployment to the EC2 instance. 
When a new change is detected in the repository, the YAML workflow automatically connects to the EC2 instance via SSH, updates the portfolio's source code, 
and reflects the changes on the live website.
          
This setup ensures that my portfolio remains up to date without the need for manual intervention, 
and it demonstrates my ability to use cloud infrastructure and automation effectively.

![project1](https://github.com/user-attachments/assets/fdd374c0-d9a7-468e-be5b-b9d91977ccf1)
![Screenshot 2024-11-29 225119](https://github.com/user-attachments/assets/cea17b4d-e954-4163-869f-e80e9c724f94)
![Screenshot 2024-11-29 225206](https://github.com/user-attachments/assets/411fd8b5-c164-43ae-a309-cfa44df7d837)


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
