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
    }
}
