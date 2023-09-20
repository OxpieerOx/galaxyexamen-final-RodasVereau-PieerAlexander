pipeline {
    agent any

    stages {
        stage('build') {
            agent {
                docker { image 'maven:3.6.3-openjdk-11-slim'}
            }
            steps {
                echo 'Llegué a la etapa de construcción'
            }
        }

        // stage('SonarQube') {
        //     steps {
        //         script {
        //             def scannerHome = tool 'scanner-default'
        //             withSonarQubeEnv('sonar-server') {
        //                 sh "${scannerHome}/bin/sonar-scanner \
        //                     -Dsonar.projectKey=exammaven01 \
        //                     -Dsonar.projectName=exammaven01 \
        //                     -Dsonar.sources=src/main/kotlin \
        //                     -Dsonar.java.binaries=build/classes \
        //                     -Dsonar.tests=src/test/kotlin"
        //             }
        //         }
        //     }
        // }
    }
}
