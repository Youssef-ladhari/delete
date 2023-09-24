pipeline {
    agent any
    
    stages {
        stage("Hello") {
            steps {
                echo "Pipeline Says hello"
            }
        }
        
        stage("Git Pull") {
            steps {
                echo "Git pull";
                    git branch :'main',
                    url : "https://github.com/Youssef-ladhari/delete.git"
            }
        }
        
        stage("Maven") {
            steps {
                sh """mvn -version"""
            }
        }
    }
}
