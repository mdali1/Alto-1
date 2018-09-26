pipeline {
    agent any
    tools { 
        maven 'Maven Tool'
	}
    

    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh 'mvn clean compile'
		    echo 'compile stage is completed here'
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
		    echo 'Testing stage ins copmpleted here'
                
            }
        }


   
    }
}
