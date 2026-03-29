pipeline {
  agent {
    docker { image 'ubuntu/nginx:1.24-24.04_beta' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'nginx -v'
      }
    }
    agent {
    docker { image 'node:16-alpine' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'node --version'
      }
    }
    agent {
    docker { image 'httpd:2.4' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'httpd -version'
      }
    }
  }
}
