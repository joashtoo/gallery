pipeline{
    agent any
    tools{
        gradle 'gradle'
    }
    stages{
        stage('Clone Code'){
            steps{
                git branch: 'master' , url: 'https://github.com/joashtoo/gallery.git'
            }
        }
        
        stage('Build Code'){
            steps{
                sh 'gradle build'
            }
        }
        
        stage('Test Code'){
            steps{
                sh 'gradle test'
            }
        }
    }
}