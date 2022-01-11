pipeline{
    agent any
    stages{
        stage('python'){
            agent {
        docker { image 'python:latest' }
              }
            steps{
                sh "python --version"
            }
        }
        stage('groovysh'){
            agent {
                docker {image 'groovy:latest'}
            }
                steps{
                    sh "groovysh --version"
                }
            }
        }
    }
