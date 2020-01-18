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
            }
        }
        stage('Build'){
            steps{ echo "Build is over"
            }
        }
            stage('Test'){
                steps{echo "Test is over"
                }
            }
        }
    }
