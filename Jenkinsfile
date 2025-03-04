pipeline {
  agent { label 'linux' }
  stages {
    stage('Clone Repo') {
      git 'https://github.com/droske00/JenkinsAnsible'
    }
    stage('httpd') {
      steps {
        sh 'ansible-playbook -i inventory httpd.yml'
      }
    }
  }
}
  
