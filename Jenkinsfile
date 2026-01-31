pipeline{
    agent any
    stages{
        stage("TEST"){
            steps{
                sh("sudo yum install python3-pip* -y")
            }
        }
        stage("DEV"){
            steps{
                sh ("pip --version")
            }
        }
        stage("DEV1"){
            steps{
                sh("sudo pip3 install ansible")
            }
        }
        stage("PRD"){
            steps{
                sh("ansible --version")
            }
        }
        stage("POSTPRID"){
            steps{
                sh("ansible localhost -m shell -a 'uptime'")
            }
        }
        
            
    }
    post{
        always{
            echo "Needd to check build success r not"
        }
        failure{
            echo "Build is failed"
        }
        success{
            echo "Build is success"
        }
    }
}
