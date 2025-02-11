pipeline {
    agent any

    stages {
        stage('Git clone') {
            steps {
                git branch: 'master', url: 'https://github.com/Akash-coder8147/Amazon'
            }
        }

        stage('Clean') {
            steps {
                sh 'mvn clean'
            }
        }
      

        stage('compile') {
            steps {
              
                  sh 'mvn compile'
            }
        }
        

        stage('test') {
            steps {
             
                  sh 'mvn test'
            }
        }
        

        stage('build') {
            steps {
            
                  sh 'mvn clean install'
            }
        }
       
    
}

}
