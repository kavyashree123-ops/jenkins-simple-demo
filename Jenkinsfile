pipeline {
  agent any

  stages {

    stage('Clone') {
      steps {
        git url: 'https://github.com/Sharanya21-ai/jenkins_simple_demo.git',
            branch: 'main'
      }
    }

    stage('Run Python Script') {
      steps {
        sh 'python3 --version'     // optional: check python
        sh 'python3 python.py'     // runs your python file
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
