pipeline {
  agent any

tools{
  maven 'Maven3'
  jdk 'JDK_21'
  }
  
  stages{
    stage ('checking'){
      steps{
        git branch:'main', url: 'https://github.com/S-Vilka/InClassAssignmmentWeek6.git'
      }
    }
  
    stage ('build'){
      steps{
        sh 'mvn install'
      }
    }

    
  }
}
