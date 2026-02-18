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
      Steps{
        sh'chmod +x script.sh'
        sh'./script.sh'
      }
    }
  }
}
      
    
