pipeline {
    agent any 
    stages {
        stage('clone repo to remote host') { 
            steps {
               echo 'push repo to remote host'
                sh 'ssh -i ~/ggg.pem -o StrictHostKeyChecking=no ubuntu@13.234.118.115 sudo rm -rf /var/www/html/'
                sh 'ssh -i ~/ggg.pem -o StrictHostKeyChecking=no ubuntu@13.234.118.115 sudo git clone https://github.com/jojojoseff/htmltestsite.git /var/www/html/'
            
            }
        }

    }
}
