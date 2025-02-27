pipeline {
  agent any
  stage ('checking'){
  steps{
    git branch:'main', url: 'https://github.com/S-Vilka/InClassAssignmmentWeek6.git'
    
    }
  }
  
  stage ('build'){
    steps{
      sh 'mvn clean install'
    }
    
  }
}
