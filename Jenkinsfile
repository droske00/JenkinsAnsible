pipeline {
  agent { label 'linux' }
  stages {
    stage('httpd') {
      steps {
        sh 'ansible-playbook -i webservers httpd.yml'
      }
    }
  }
}
  
