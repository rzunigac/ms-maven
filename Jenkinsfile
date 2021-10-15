pipeline {
    agent any

    tools {
        maven 'Maven'
    }
  
    stages {
        stage('initial'){
            steps{
             sh '''
              echo "PATH = ${PATH}"
              echo "M2_HOME = ${M2_HOME}"
              '''
            }
        }
        
        stage('Compile'){
            steps{
                sh 'mvn clean compile -e'
            }
        }
        
    }
    
           
}
