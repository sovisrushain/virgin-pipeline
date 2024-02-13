pipeline {
    agent any
    stages {
        stage("Clean Up") {
            steps {
                deleteDir()
            }
        }
        stage("Clone Repo") {
            steps {
                sh "git clone https://github.com/sovisrushain/virgin-pipeline.git"
            }
        }
        stage("Build") {
            steps {
                dir("Test") {
                    sh "pwd"
                    sh "mvn clean install"
                }
            }
        }
    }
}