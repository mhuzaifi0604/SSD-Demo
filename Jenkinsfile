flag = false
pipeline {
  agent any
  environment {
    NEW_VERSION = '1.3.0'
  }
  stages {
    stage('Build') {
      steps {
         echo 'Building..'
        // Here you can define commands for your 
        echo "building version ${New_VERSION}"
      }
    }
    stage('Test') {
      when {
        expression {
          flag == true
        }
      }
      steps {
        echo 'Testing..'
        // Here you can define commands for your tests
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
        // Here you can define commands for your deployment
      }
    }
  }
  post {
    // the conditions after build
    always {
      echo 'Always run this step'
    }
    failure {
      echo 'Failed, but run this step'
    }
  }
}
