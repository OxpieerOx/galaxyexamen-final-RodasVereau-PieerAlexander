pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                checkout scm
            }
        }

          stage('build') {
            steps {
                echo 'Llegué a la etapa de construcción'
                // Puedes agregar más mensajes de registro si es necesario
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
