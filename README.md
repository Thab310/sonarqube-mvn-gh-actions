# sonarqube-mvn-gh-actions

### Prerequesites
1. Create SonarQube server
2. Initialize a simple hello-world springboot application
### What is SonarQube?
It is a self-managed tool that helps you deliver clean code by automating code reviews.
### Steps
1. Log into the server and generate and copy token
2. Create a github repository and create repository action secrets.

   ```bash
   SONAR_TOKEN 
   ```

   ```bash
   SONAR_HOST_URL 
   ```
   `Note`: These will be used to authenticate your sonar server, in our case, its a an ec2 running on aws.   
3. Create .github/workflows/maven.yml workflow on your root directory of your source code

4. Copy and update the workflow from SonarQube website: https://docs.sonarsource.com/sonarqube/latest/devops-platform-integration/github-integration/

5. Push code into github 