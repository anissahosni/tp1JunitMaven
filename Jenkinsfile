pipeline {
   
    agent any
   
    stages {

        stage('get code from github + web hook pipeline') {
            steps {
                echo 'Pulling...';
                git branch: 'master',
                url : 'https://github.com/PYTHONRA/tp1JunitMaven.git';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}