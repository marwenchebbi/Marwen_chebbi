pipeline {
    agent any 
    stages {
        stage('Azure Login') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'azure-cred', 
                                                usernameVariable: 'AZURE_USER', 
                                                passwordVariable: 'AZURE_PASS')]) {
                    sh '''
                    az login -u $AZURE_USER -p $AZURE_PASS
                    az account show
                    '''
                    echo "Logged in successfully ."
                }
            }
        }
    }
}
