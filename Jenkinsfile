stage "unit test"
sh "pwd"
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


parallel (
  windows: { node {
    sh "echo building on windows now"

 }},
  mac: { node {
    sh "echo building on mac now"
}})
