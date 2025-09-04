pipeline {
  agent any
  stages {
    stage('Fetch Code') {
      steps {
        git(url: 'https://github.com/AnmolSingh8858/jenkins-devops1.git', branch: 'main', poll: true)
      }
    }

    stage('Apache install') {
      steps {
        sh 'sudo install apache2 -y'
      }
    }

    stage('deploy App') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}