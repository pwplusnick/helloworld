pipeline {
    agent any
   
    stages {
	stage('\u27A1 ') {
            steps {
                sh '''sudo apt-get -y install git gcc'''
            }
        }
        stage('\u27A1 Build') {
            steps {
                sh '''cc $WORKSPACE/hello.c -o $WORKSPACE/hello'''
            }
        }
        stage('\u27A1 Run') {
            steps {
                sh '$WORKSPACE/hello'
            }
        }
        
    }
    post {
        always {
            sh '''rm -fr $WORKSPACE/*'''
        }
    }
}

