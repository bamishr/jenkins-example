pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                 
                    sh 'mvn clean compile'
					sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
                
            }
        }


        stage ('Deployment Stage') {
            steps {
               
                    sh 'mvn deploy'
                
            }
        }
    }
}