pipeline{
    agent any

    stages{
        stage ('Compile Stage'){
            steps {
                withMaven(maven : 'default'){
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage'){
            steps {
                withMaven(maven : 'default'){
                    sh 'mvn test'
                }
            }
        }

        stage ('Package Stage'){
            steps {
                withMaven(maven : 'default'){
                    sh 'mvn package'
                }
            }
        }
    }
}