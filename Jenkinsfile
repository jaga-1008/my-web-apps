pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo "build with maven"
            }
        }

        stage('upload to nexus'){
            steps{
                echo "upload to nexus"
            }
        }

        stage('deploy to dev'){
            when {
              branch 'dev'
            }

            steps{
                echo "deploy to dev"
            }
        }

        stage('deploy to test'){
            when {
              branch 'test'
            }

            steps{
                echo "deploy to test"
            }
        }

        stage('deploy to master'){
            when {
              branch 'master'
            }
            
            steps{
                echo "deploy to master"
            }
        }
    }
}