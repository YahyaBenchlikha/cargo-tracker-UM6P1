pipeline {
    agent any

    triggers {
        githubPush()   
    }

    stages {

        stage('Clone') {
            steps {
                git branch: 'develop', url: 'https://github.com/YahyaBenchlikha/cargo-tracker-UM6P1.git'
            }
        }

        stage('Build & Test with Coverage') {
            steps {
                echo 'hello '
            }
        }

    }
//
    post {
        success {
            echo 'Build et analyse terminés avec succès !'
        }
        failure {
            echo 'Échec du build ou des tests.'
        }
    }
}
