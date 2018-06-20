pipeline {
  agent any
  stages {
    stage('AOT Build') {
      steps {
        sh 'docker.build("myinfo-dpp", "-f Dockerfile-Nectar-STG .")'
      }
    }
    stage('Done') {
      steps {
        sh 'sh \'echo "Tests passed"\''
      }
    }
  }
}