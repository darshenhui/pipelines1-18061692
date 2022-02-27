pipeline {
         agent any
         stages {
                 stage('Stage 1- 18061692') {
                 steps {
                     echo 'Stage 1- Completed- 18061692'
                 }
                 }
                 stage('Stage 2- 18061692') {
                 steps {
                    input('Do you want to proceed?')
                 }
                 }
                 stage('Stage 3- 18061692') {
                 when {
                       not {
                            branch "master"
                       }
                 }
                 steps {
                       echo "Hello"
                 }
                 }
                 stage('Stage 4- 18061692') {
                 parallel { 
                            stage('Unbuntu Images') {
                           steps {
                                echo "Running the unit test..."
                           }
                           }
                            stage('Stage 5- 18061692') {
                              agent {
                                    docker {
                                            reuseNode true
                                            image 'ubuntu:18.04'
                                           }
                                    }
                              steps {
                                echo "work released- 18061692"
                              }
                           }
                           }
                           }
              }
}
