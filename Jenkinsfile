#!/usr/bin/env groovy

/// Commit0 Code 123

pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', 
                          branches: [[name: '*/Branch2']], 
                          doGenerateSubmoduleConfigurations: false, 
                          extensions: [], submoduleCfg: [], 
                          userRemoteConfigs: [[credentialsId: '202afffc-47cc-4695-a395-8c5e087e4d22', 
                                              url: 'https://github.com/lokeshreddy470/Multi_branch_project.git']]])
            }
        }
        stage('Build') { 
            steps { 
                echo " This is Build Stage"
            }
        }
        stage('Test'){
            steps {
                echo "This is a Test Stage" 
            }
        }
        stage('Deploy') {
            steps {
                echo "This is a Deploy Stage"
            }
        }
    }
}
