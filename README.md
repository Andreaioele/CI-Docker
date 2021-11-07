# Create CI Environment using Github Actions and Docker
#### This guide help you to init a java project to run test in CI. This approach is very useful to automate test process and it tempts you to write clean code. Follow these step to start coding.

## 1 - Before start
Ensure you to create Docker Repository from your Docker Hub. Choose a name and create repo

##### build the project

    mvn build

##### build Docker image called java-app. Execute from root

    docker build -t java-app .
    
##### PUSH docker image 

    docker tag java-app <YOUR-REPO-NAME>:java-1.0
    
##### PUSH docker image to Docker Hub
    
    docker push <YOUR-REMPO-NAME>/demo-app:java-1.0
    
## 2 - Setup/edit Github Actions
<ul>
    <li>Create a <code>.github/workflows</code> directory in your repository on GitHub if this directory does not already exist. </li>
    <li>In the <code>.github/workflows</code> directory, create a file named <code>github-actions-demo.yml</code></li>
    <li>Paste your custom workflow and save</li>
</ul>


    
