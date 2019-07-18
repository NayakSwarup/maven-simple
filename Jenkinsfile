pipeline{
  agent any
  tools{
      maven 'Maven'
  }
    stages{
      stage('checkout source code from repository'){
            steps{
                git 'https://github.com/NayakSwarup/maven-simple'
            }
        }
        stage('compiling  the source code'){
            steps{
                bat'mvn -v'
            }
        }
        
       stage('packaging  the source code'){
            steps{
                bat'mvn clean package'
            }
        }
        }
    }
