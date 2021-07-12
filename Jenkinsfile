pipeline{
    agent any
    stages{
        stage('build'){
            when {
              branch 'dev'
            }
            steps{
                echo "build with maven"
            }
        }

        stage('upload to nexus'){
            when {
              branch 'dev'
            }
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