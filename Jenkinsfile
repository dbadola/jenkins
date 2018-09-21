pipeline {
  agent {
    node {
      label 'master'
    }
  }
  stages {
        stage('terrafrom started') {
            steps {
                sh 'echo "Started...!" '
            }
        }
        stage('git clone') {
            steps {
                sh 'sudo rm -r *; sudo git clone https://github.com/dbadola/jenkins.git'
            }
        }
        stage('terraform init') {
            steps {
                ssh 'sudo /home/ec2-user/terraform plan ./jenkins'
            }
        }
    }
}
