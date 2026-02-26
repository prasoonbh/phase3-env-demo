/* this is the example of enviroment variable
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

} */


pipeline {

    agent any

    paramenters {
        string(
            name: 'ENV' ,
            defaultValue: 'dev'
            description: 'Enviroment'
        )
    }

    stages {

        stage('Show enviroment'){
            steps {
                echo "Deploying to ${params.ENV}"
            }
        }
    }
}