pipeline {

    agent any

    environment {
        APP_NAME = "myapp"
        VERSION = "1.0"
    }

    stages {

        stage('Print Variables') {
            steps {

                echo "App Name: ${env.APP_NAME}"
                echo "Version: ${env.VERSION}"

            }
        }

    }

}