pipeline {
agent any
stages {
stage('Build') {
steps {
echo 'Building..'
// Here you can define commands for your build
}
}
stage('Test') {
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
  echo 'writing post to jenkins file'
  always {
    echo 'writing always to jenkins file'
  }
  failure {
    echo 'writing failure to jenkins file'
  }
}
}
