pipeline {
  agent {
    node {
      label 'master'
    }
  }
  stages {
        stage('terrafrom started') {
            steps {
                echo "Started...!"
            }
        }
        stage('terrafrom version') {
            steps {
                echo "terraform --version"
            }
        }
    }
}
