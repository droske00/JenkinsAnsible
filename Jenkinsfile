pipeline {
  agent { label 'linux' }
  stages {
    stage('httpd') {
      steps {
        sh 'ansible-playbook -i inventory/node1 playbooks/httpd.yml'
      }
    }
  }
}
  
