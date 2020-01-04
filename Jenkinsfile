pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'Java8'
    }
    
stages { 
    stage('Clone'){
        steps{
            git credentialsId: '517afbfd-951a-431e-aa42-88f7c78f730b', url: 'https://github.com/boopathyvignesh/NewMavenMyApp.git'
        }
    }
    
    stage ('Build'){
    
        steps {
            sh 'mvn clean package'
        }
    }
    stage ('Deploy'){
    
        steps{
            sh "echo deploy success"
            
        }
    }
    }
}
