pipeline{
    agent { label 'controlnode'}
    stages{
        stage ('Sorce Code'){
            steps {
                git branch:'main', url:'https://github.com/pixelswapnil13/BasicNodeJsProgramme.git'
            }
        }
        stage ('Install dependancies'){
            steps {
                sh 'npm install'
            }           
        }
        stage ('Build the project'){
            sh 'npm run build'
        }
    }
}