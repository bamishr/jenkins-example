pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                 
                    echo "sh 'mvn test'"
					
                
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
		stages {
        stage ('Integration Stage') {

            steps {
                 
                    echo "sh 'mvn test'"
					
                
            }
        }
		stages {
        stage ('Promotion Stage') {

            steps {
                 
                    echo "sh 'mvn test'"
					
                
            }
        }
    }
	}
}
}