pipeline {
  agent { label 'linux' }
  stages {
   /* stage('Clone Repo') {
      steps {
         sh 'git clone https://github.com/droske00/JenkinsAnsible.git'
      }
    } */
    stage('httpd') {
      steps {
        sshagent(['3']) 
        sh 'ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook -i inventory httpd.yml'
      }
    }
  }
}
  
