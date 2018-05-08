# pipeline-demo
Demo of pipelines in Jenkins

## Running Jenkins locally

https://github.com/jenkinsci/docker/blob/master/README.md

Just for testing:
  docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins:lts

This will automatically create a 'jenkins_home' docker volume on the host
machine, that will survive the container stop/restart/deletion:
  docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts

- Fork this project

- Log in with the random administrative password printed to the Docker log.
- Install selected plugins
- Continue as admin
- Start using Jenkins
- Create a new item -> pipeline project
- Pipeline script from SCM
- Add your repository URL (https)
- Save
- Build Now

Optional
- Install Blue Ocean plugin to view the parallel part
