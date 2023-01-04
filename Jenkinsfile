pipeline{
    agent {label 'OPENJDK-JDK'}
    stages{
        stage('GIT'){
            steps{
                git url : 'https://github.com/mallojuashok/js-e2e-express-server.git' , branch: 'main'
            }
        }
        stage(BUILD){
            steps{
                sh 'npm install' 
                
            }
        }
        stage(START){
            steps{
                sh 'npm start'
            }
        }
    }
}
