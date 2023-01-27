pipeline {
  agent any
  
  stages {
    
    stage ('Build Docker Image'){
      steps {
        script{
          dockerapp = docker.build("denispetraquim/kube-news:${env.BUILD_ID}", '-f ./Dockerfile .')
        }
      }
    }
  }
