pipeline {
  agent { label 'linux' }
      environment {
        MY_CREDENTIALS = credentials('1')  // ID kredencijala
    }
  stages {
   /* stage('Clone Repo') {
      steps {
         sh 'git clone https://github.com/droske00/JenkinsAnsible.git'
      }
    } */
    stage('httpd') {
      steps { 
        sh """
             ansible-playbook -i inventory httpd.yml --extra-vars "ansible_user=${MY_CREDENTIALS_USR} ansible_password=${MY_CREDENTIALS_PSW}"
         """
      }
    }
  }
}
  
