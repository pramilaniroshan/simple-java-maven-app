pipeline {

agent any
    options {
        skipStagesAfterUnstable()
    }

    stage {
        stage('Build') {
            steps {
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                echo "test"
            }
            post {
                always {
                    echo "post"
                }
            }
        }
        stage('Deliver') { 
            steps {
                echo "Deliver"
            }
        }
    }
}
