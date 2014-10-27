# Experiments with the code from the dockerbook

 * http://dockerbook.com/code/5/jenkins/Dockerfile
 * http://dockerbook.com/code/5/jenkins/dockerjenkins.sh

    docker build -t jenkins .
    docker run --publish 8080:8080 --name jenkins --privileged --detach jenkins


## Jenkins job

Use custom workspace:

    /tmp/jenkins-buildenv/${JOB_NAME}/workspace

Git url:

    https://github.com/jamtur01/docker-jenkins-sample.git

Execute shell — http://dockerbook.com/code/5/jenkins/jenkins_single_shell_step

Publish JUNIT test result report:

    spec/reports/*.xml
