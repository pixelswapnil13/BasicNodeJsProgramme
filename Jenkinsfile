pipeline{
    agent{ label 'JDK11'}
    stages{
        stage('Source Code'){
            steps{
                git branch:'declarative', url: 'https://github.com/pixelswapnil13/BasicNodeJsProgramme.git'
            }
        }
        stage('Install dependancies'){
            steps{
                sh 'npm install'
            }
        }
        stage('Build the project'){
            steps{
                sh 'npm run build'
            }
        }
        stage('Build the project'){
            steps{
                sh 'npm run test'
            }
        }
        stage('Archiving the project'){
            steps{
                sh 'npm pack'
            }
        }

    }
}