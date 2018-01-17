pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                 
                    sh "'${M2_HOME}/bin/mvn' -Dmaven.test.failure.ignore clean package\"\n"
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