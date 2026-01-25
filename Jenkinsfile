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
    }
}
