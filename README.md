UDACITY CLOUD ENGINEER PROJECT 04 - Build CI/CD Pipeline for Blue/Green Deployment

Github URL: https://github.com/dchaves30/Continuous-Integration-and-Continuous-Deployment
S3 Bucket URL: https://udacity-project04.s3-us-west-2.amazonaws.com/index.html


Contents of the zip file:

- index.html : html file copied to the S3 bucket from the Jenkins BlueOcean pipeline
- jenkinsfile : jenkins file with the instructions for project 04
- README.md : This Document

Folders: 
- Screenshots : Contains 3 folders with screeshots for each required item for each section of the project rubric:
    - AWS Setup
        - EC2_Instance.PNG : Shows the running EC2 instance information
        - EC2_Instance_SSH_Access.PNG : Shows the SSH access using Putty
        - groups.PNG : Shows the group created for the project 04
        - user.PNG - shows the non-root user created for the project 04

    - Running Jenkins
        - Jenkins_BlueOcean.png : Shows the blueocean interface
        - Jenkins_BlueOcean_Pipeline_01.png: Show a 1 step pipeline
        - Jenkins_BlueOcean_SideBar.PNG - Shows the Blueocean sidebar in the jenkins interface
        - Jenkins_Login.png : Jenkins Login Page

    - Working Pipeline
        - index_file_URL.png : URL for S3 bucket html file
        - Jenkins_BlueOcean_Pipeline_Copy_to_S3.png : Pipeline showing copy to S3 step
        - jenkinsfile_with_steps_and_credentials.png : jenkinsfile source code on github
        - Pipeline_with_LINT_step.png: Pipeline step showing the usage of LINT
