pipeline{
    agent any

    stages{
        stage ('Compile Stage'){
            withMaven(maven : 'default'){
                sh 'mvn clean compile'
            }
        }

        stage ('Testing Stage'){
            withMaven(maven : 'default'){
                sh 'mvn test'
            }
        }


        stage ('Deployment Stage'){
            withMaven(maven : 'default'){
                sh 'mvn deploy'
            }
        }
    }
}