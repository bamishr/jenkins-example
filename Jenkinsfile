pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                 
                    sh "'${M2_HOME}/bin/mvn' -Dmaven.test.failure.ignore clean package\"\n"
					
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    echo "sh 'mvn test'"
                
            }
        }


        stage ('Deployment Stage') {
            steps {
               
                    echo "sh 'mvn deploy'"
                
            }
        }
    }
}