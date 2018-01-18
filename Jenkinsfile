pipeline {
    agent any

	
    stages {
        stage ('Compile Stage') {

            steps {
                 
                    echo "sh 'mvn test'"
					bat 'mvn clean compile'
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    echo "sh 'mvn test'"
                    bat 'mvn test'
            }
        }


        stage ('Deployment Stage') {
            steps {
               
                    echo "sh 'mvn deploy'"
                    bat 'mvn install'
            }
        }
    }
}