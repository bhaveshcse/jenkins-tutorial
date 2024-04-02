## Jenkins-tutorial
Jenkins is an open source automation server. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration, and continuous delivery. It is a server-based system that runs in servlet containers such as Apache Tomcat.

# Jenkins Pipeline 
(or simply "Pipeline" with a capital "P") is a suite of plugins which supports implementing and integrating continuous delivery pipelines into Jenkins.
A continuous delivery (CD) pipeline is an automated expression of your process for getting software from version control right through to your users and customers. Every change to your software (committed in source control) goes through a complex process on its way to being released. This process involves building the software in a reliable and repeatable manner, as well as progressing the built software (called a "build") through multiple stages of testing and deployment.

# Declarative versus Scripted Pipeline syntax
A Jenkinsfile can be written using two types of syntax — Declarative and Scripted.
Declarative and Scripted Pipelines are constructed fundamentally differently. 

Declarative Pipeline is a more recent feature of Jenkins Pipeline which: provides richer syntactical features over Scripted Pipeline syntax, and is designed to make writing and reading Pipeline code easier.

Many of the individual syntactical components (or "steps") written into a Jenkinsfile, however, are common to both Declarative and Scripted Pipeline. 

# Declarative pipeline
<br>pipeline{<br>
    agent any<br>
    stages{<br>
        <br>stage("code build"){
            <br>steps{
                <br>echo "code build"
            <br>}
        <br>}
            <br>    stage("code push"){
            <br>steps{
                <br>echo "code push"
            <br>}
        <br>}
            <br>    stage("code deploy"){
            <br>steps{
                <br>echo "code deploy"
            <br>}
        <br>}
    <br>}
}
