#!/usr/bin/env groovy
properties([
           [$class: 'GithubProjectProperty', 
            displayName: '', 
            projectUrlStr: 'https://github.com/lokeshreddy470/Multi_branch_project.git/'],
            pipelineTriggers([githubPush()])
])

pipeline {
    agent any

    stages {
        stage('Build') { 
            steps { 
                echo " This is Build Stage"
            }
        }
        stage('Test'){
            steps {
                echo "This is a Test Stage" 
                sh 'ls'
                sh 'java -version'
            }
        }
        stage('Deploy') {
            steps {
                echo "This is a Deploy Stage"
                sh 'pwd'    
                   
            }
        }
    }
}
