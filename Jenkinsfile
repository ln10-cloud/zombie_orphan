pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Stage build"'
        sh 'cd $WORKSPACE && ls -al'
        sh 'gcc zombie.orphan.c -o zombie.out && chmod u+x zombie.out && ./zombie.out'
      }
    }
    stage('Unit Test') {
      steps {
        echo 'Stage unit test'
      }
     }
    stage('Interface Test') {
      steps {
        echo 'Stage interface test'
      }
    }
    stage('System Test') {
      steps {
        echo 'Stage System test'
      }
    }
    stage('Delivery') {
      steps {
        sh 'echo "Stage Delivery"'
        sh 'echo "Push image to docker repo"'
      }
    }
  }
}
