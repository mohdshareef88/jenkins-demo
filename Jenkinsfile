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
  }
}
