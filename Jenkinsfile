pipeline { 
    agent any 
    tools{
        maven 'LOCALMAVEN'
        jdk 'LOCAL_JDK'
    }
    stages {
        stage('clean') { 
            steps { 
                bat 'mvn clean' 
            }
        }
        stage('test'){
            steps {
                bat 'mvn test'
            }
        }
        stage('package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
