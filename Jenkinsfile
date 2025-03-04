pipeline {
  agent { label 'linux' }
  stages {
    stage('httpd') {
      steps {
        sh 'ansible-playbook -i node1 httpd.yml'
      }
    }
  }
}
  
