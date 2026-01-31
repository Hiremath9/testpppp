pipeline{
    agent any
    stages{
        stage("test"){
            when{
                changeset "test"
            }
            steps{
                sh ("uname")
            }
        }
        stage("test2"){
            when{
                changeset "test"
            }
            steps{
                sh("uname -r")
            }
        }
    }
}
