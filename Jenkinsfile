pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat(script: 'cd /demo', encoding: 'utf8', label: 'Go to demo project')
        bat(script: 'mvn clean', encoding: 'utf8', label: 'Clean')
        bat(script: 'mvn install', encoding: 'utf8', label: 'Install')
        bat(script: 'cd /groovy-tutorial', encoding: 'utf8', label: 'Go to groovy-tutorial project')
        bat(script: 'mvn clean', encoding: 'utf8', label: 'Clean')
        bat(script: 'mvn install', encoding: 'utf8', label: 'Install')
      }
    }

    stage('Test') {
      steps {
        echo 'Chay trong test'
      }
    }

    stage('Deploy') {
      steps {
        echo 'hay trong deploy'
      }
    }

    stage('Finish') {
      steps {
        echo 'Finished'
      }
    }

  }
}