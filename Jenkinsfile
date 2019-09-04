pipeline {
  agent { docker { image 'python:3.5.1' } }
  stages {
    stage('build') {
      steps {
        sh 'pip install --upgrade pip'
        sh 'pip install -r requirements.txt'
      }
    }
    stage('test') {
      steps {
        sh 'python --version'
        sh 'python test.py'
      }   
    }
  }
}
