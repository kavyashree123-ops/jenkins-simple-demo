pipeline {
  agent any

  stages {

    stage('Clone') {
      steps {
        git url: 'https://github.com/kavyashree123-ops/jenkins-simple-demo.git',
            branch: 'main'
      }
    }

    stage('Verify Files') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Run Python Script') {
      steps {
        sh 'python3 --version'
        sh 'python3 python.py'
      }
    }

    stage('Run Shell Script') {
      steps {
        sh 'chmod +x script.sh'
        sh './script.sh'
      }
    }
  }
}
