pipeline {
  agent {
    docker { image 'centos/httpd' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'httpd --version'
      }
    }
  }
}
