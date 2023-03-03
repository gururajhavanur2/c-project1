pipeline {
    agent any 
    stages {
        stage('parallel') {
            when {
                branch 'master'
            }
            parallel {
                stage('STAGE-1') {
                    steps{
                        sh "echo STAGE-1 executes if branch is master"
                    }
                }

                stage('STAGE-2'){
                    steps{
                        sh "echo STAGE-2 executes if branch is master"
                    }
                }
            }    
        }    
    }
}
