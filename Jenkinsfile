pipeline {
    agent any
    stages {
        stage('Generate') {
            steps {
                echo "Generating....";
             }
        }
        stage('build') {
            steps {
                echo "building....";
              }
        }
        stage('Test') {
            steps {
                echo "Testing....";
              }
        }
        stage('Deploy') {
            steps {
                echo "Deploying....";
              }
        }
    }
    post {
         always {
             echo 'This will run always'
         }
         success {
             echo 'This will run only if successful'
         }
         failure {
             echo 'This will run only if failed'
         }
         unstable {
             echo 'This will run only if the run was marked as unstable'
         }
         changed {
             echo 'This will run only if state of Pipiline has changed'
             echo 'For example, if the Pipeline was previously failing but is now successful'
         }
     }
}
