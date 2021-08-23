node {
    stage('Clonacion Repositorio') {
        git branch: 'master',
            credentialsId: 'githubssh',
            url: 'git@github.com:ContardoRM/DVWA.git'

        sh "ls -lat"
        
    }
    stage('Test Unitarios') {
        sh 'echo "Tests passed Hola mundo"'
    }
    stage('Analisis de Codigo con Sonar') {
        sh 'java -version'
    }
    stage('Deploy sobre EC2') {
        sh 'echo "test"'
    }
    stage('Send slack notification') {
         slackSend color: 'good', message: 'Message from Jenkins Pipeline'
    }
}
