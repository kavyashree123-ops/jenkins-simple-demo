pipeline {
  agent any 
  
  stages{
    
    stages('clone'){
      steps{
        git url:'https://github.com/kavyashree123-ops/jenkins-simple-demo.git',
          branch: 'main'
      }
    }

    stage('Run Script'){
      steps{
        sh'chmod +x script.sh'
        sh'./script.sh'
      }
    }
  }
}
      
    
