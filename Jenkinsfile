pipeline {
    agent any
    stages {
        stage("Clone Repo"){
            steps {
                git branch: 'master', url: 'https://github.com/oscar066/java-todo.git'
            }
        }
        stage("Build repo"){
            steps {
                sh "./gradlew clean build "
            }
        }
        stage("Test Code"){
            steps {
                sh "./gradlew test"
            }
        }
    }
}