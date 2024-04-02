pipeline {
  
    agent {
        label 'Java-Node'
    }
    
    tools{
        maven "maven 3.9.6"
    }

    stages {
        stage('Clone') {
            steps {
               git '<Github Path>'
            }
        }
        stage('Build') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
