pipeline {
    agent any
      tools {nodejs "Node installation"}
     stages {
        stage('Build') {
            steps {
                echo 'npm install'
            }
        }
        stage('Run collection') { 
            steps {
                sh 'node --version'
                sh 'newman --version'
                sh './jenkins/scripts/test.sh'
           
            }
        }
    }
}
