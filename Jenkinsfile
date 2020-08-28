pipeline {
    agent any

    stages {

        stage('FrontEnd Build') {
        
            steps {
                nodejs('NodeJS 12.14.0') {
                    sh label: '', script: '''
                    lerna exec -- npm i && lerna link
                    npm run build
                    '''
                }
            }

}
