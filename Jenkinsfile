pipeline{
    agent any
    stages {
    
        stage('Setup Python Virtual ENV'){
       
      steps  {
            sh '''
            cd ./scripts
            chmod +x envsetup.sh
            ./envsetup.sh
            '''}
        }
        stage('Setup Gunicorn Setup'){
            steps {
                sh '''
                cd ./scripts
                chmod +x gunicorn.sh
                ./gunicorn.sh
                '''
            }
        }
        stage('setup NGINX'){
            steps {
                sh '''
                cd ./scripts
                chmod +x nginx.sh
                ./nginx.sh
                '''
            }
        }
    }
}
