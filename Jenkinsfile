pipeline {
  agent any
  stages {
    stage('Deploy Apigee') {
      parallel {
        stage('Deploy Apigee') {
          steps {
            git(url: 'https://github.com/swilliams11/apigee_build_jenkins_example3.git', branch: 'master')
          }
        }
        stage('maven') {
          steps {
            sh 'mvn install'
          }
        }
      }
    }
  }
}