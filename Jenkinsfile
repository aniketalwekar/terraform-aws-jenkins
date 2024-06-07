
pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                script {
                    def exampleMap = [
                        Id: 'testpipeline',
                        url: 'https://github.com/aniketalwekar/terraform-aws-jenkins.git'
                    ]
                    // Rest of your script
                }
            }
        }
    }
}
        stage('Terraform Init'){
            steps{
                sh 'terraform init'
            }
        }
        stage('Terraform Plan'){
            steps{
                sh 'terraform plan'
            }
        }
         stage('Terraform Apply'){
            steps{
                sh 'terraform apply --auto-approve'
            }
        }
        // stage('Terraform Destroy'){
        //     steps{
        //         sh 'terraform destroy --auto-approve'
        //     }
        // }
}
