pipeline {
  agent { label 'linux' }
  stages {
    stage('Clone Repo') {
      steps {
         git 'https://github.com/droske00/JenkinsAnsible.git'
      }
    }
    stage('httpd') {
      steps {
        sh 'ansible-playbook -i inventory httpd.yml'
      }
    }
  }
}
  
