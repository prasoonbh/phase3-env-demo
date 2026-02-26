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

    parameters {

        string(
            name: 'ENV',
            defaultValue: 'dev',
            description: 'Environment'
        )

    }

    stages {

        stage('Show Environment') {

            steps {

                echo "Deploying to ${params.ENV}"

            }

        }

    }

}