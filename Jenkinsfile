pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                deleteDir()
                sh '''
                    git clone https://github.com/mehanarahim/project.git
                    ls -l
                '''
            }
        }
        stage('deploy'){
            steps{
                sh '''
                    cp -r project/* /var/www/html
                    ls -l /var/www/html
                '''
                   
            }
        }
       
    }
}
