pipeline {
  agent none   // no global agent

  stages {

    stage('Nginx Version') {
      agent {
        docker { image 'ubuntu/nginx:1.24-24.04_beta' }
      }
      steps {
        sh 'nginx -v'
      }
    }

    stage('Node Version') {
      agent {
        docker { image 'node:16-alpine' }
      }
      steps {
        sh 'node --version'
      }
    }

    stage('Apache Version') {
      agent {
        docker { image 'httpd:2.4' }
      }
      steps {
        sh 'httpd -version'
      }
    }
  }
}
