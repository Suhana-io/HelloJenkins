
pipeline{
    agent any
    stages{
        stage('Compile'){
            steps{
                {
                    bat 'javac src/Hello.java'
                }
            }
        }
        stage('Run'){
            steps{
                {
                    bat 'java -cp . src.Hello'
                }
            }
        }
    }
    post{
        success{
            echo  'BUILD SUCCESSFUL'
        }
        failure{
            echo 'BUILD FAILED'
        }
    }
}