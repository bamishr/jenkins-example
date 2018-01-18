pipeline {
    agent any
node {
  
  def mvnHome = tool 'M3'
  env.JAVA_HOME = tool 'JDK-1.8.0_151'
  bat "\"${mvnHome}\"\\bin\\mvn -B verify"
}
	
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
                
            }
        }


        stage ('Deployment Stage') {
            steps {
               
                    echo "sh 'mvn deploy'"
                
            }
        }
    }
}