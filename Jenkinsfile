@Library('JenkinsLiberary') _
pipeline {  
    agent any  
    stages {   
        stage('Clone') {    
            steps { 
                 git credentialsId: 'Git', url: 'https://github.com/johngit1991/puppetboard.git'
                }   
        }   
        stage('Compile') {    
            steps {     
                  sh(libraryResource('resources/input/python.sh'))
            }             
        }          
    }
}
