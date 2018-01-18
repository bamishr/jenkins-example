pipeline {
    agent any

	
    stages {
        stage ('Compile Stage') {

            steps {
                 
                    echo "sh 'mvn test'"
					env.JAVA_HOME = tool 'JDK-1.8.0_151'
					bat 'mvn clean compile'
                
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