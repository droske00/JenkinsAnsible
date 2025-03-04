pipeline {
  agent { label 'linux' }
  stages {
    stage('httpd') {
      steps {
        sh 'ansible-playbook -i invnetory/webservers httpd.yml'
      }
    }
  }
}
  
