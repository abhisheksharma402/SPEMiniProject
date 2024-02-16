pipeline{
    agent any

    tools{
        maven 'maven-3.9.6'
    }
    
    stages{
        stage('Build Maven'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/abhisheksharma402/SPEMiniProject']])
                sh 'mvn clean install'
            }
        }
    }


}
