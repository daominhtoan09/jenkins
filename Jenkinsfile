pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat(script: 'mvn -f demo clean', encoding: 'utf8', label: 'Clean')
        bat(script: 'mvn -f demo install', encoding: 'utf8', label: 'Install')
        bat(script: 'mvn -f groovy-tutorial clean', encoding: 'utf8', label: 'Clean')
        bat(script: 'mvn -f groovy-tutorial install', encoding: 'utf8', label: 'Install')
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