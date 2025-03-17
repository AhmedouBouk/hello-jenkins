pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Git checkout est automatique avec Pipeline from SCM
                echo 'Code récupéré depuis GitHub'
            }
        }
        stage('Compile') {
            steps {
                script {
                    // Compile le code Java - utilisez bat pour Windows
                    bat 'javac HelloWorld.java'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    // Exécute le code Java compilé
                    bat 'java HelloWorld'
                }
            }
        }
    }
}