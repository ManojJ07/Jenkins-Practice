pipeline {
  agent any
  stages {
    stage('Fetch Code') {
      steps {
        git(branch: 'main', url: 'https://github.com/ManojJ07/Jenkins-Practice.git')
      }
    }

    stage('Install Apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('Deploy App') {
      steps {
        sh 'sudo cp -R * /var/www/html'
      }
    }

  }
}