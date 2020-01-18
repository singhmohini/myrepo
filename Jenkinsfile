pipeline{
    agent any
    stages{
        stage('PULL from Git')
        {
            steps{
                  git 'https://github.com/singhmohini/myrepo.git'
            }
        }
          stage ('Analysis')
        {
            steps{
                sh'/opt/Maven/bin/mvn clean verify sonar:sonar -Dsonar.password=admin -Dsonar.login=admin'
                
            }
        }
        stage('Build'){
            steps{ 
              sh  '/opt/Maven/bin/mvn clean install'
            }
        }
            stage('Test'){
                steps{echo "Test is over"
                }
            }
        }
    }
