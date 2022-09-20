pipeline {
    agent any

    stages {
        stage('Gitclone') {
            steps {
                git branch: 'uber', credentialsId: 'c3934fcc-abc5-4e29-9641-cb9d245d9476', url: 'https://github.com/Anoosh02/Uber.git'
            }
        }
    }
}
