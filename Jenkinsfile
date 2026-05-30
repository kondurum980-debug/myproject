pipeline{
agent none
environment {
  environment = "dev"
  sonar_url = "https://sonar.opqtech.com"
  jfrog_url = "https://jfrog.opqtech.com"
}

stages {
  stage('Checkout') {
    steps {
      echo "this is checkout"
    }
  }

  stage('Build') {
    steps {
      echo "this build"
    }
  }

  stage('Test') {
    steps {
      echo "this is test"
    }
  }

  stage('Sonar-scan') {
    steps {
      echo "this sonar-scan"
    }
  }

  stage('Push') {
    steps {
      echo "this is push"
    }
  }

  stage('Deploy') {
    when {
  environment name: 'environment', value: 'dev'
         }

    steps {
      echo "this is deploy"
    }
  }

}
}
