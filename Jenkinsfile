pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'C:/Program Files (x86)/apache-maven-3.2.5') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'C:/Program Files (x86)/apache-maven-3.2.5') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'C:/Program Files (x86)/apache-maven-3.2.5') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}