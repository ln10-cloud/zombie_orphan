pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Stage build"'
        sh 'cd $WORKSPACE && ls -al'
        /*
        sh 'gcc zombie.orphan.c -o zombie.out && chmod u+x zombie.out && ./zombie.out'
        */
      }
    }

    stage('Test') {
      steps {
        echo 'Stage unit test'
      }
      steps {
        echo 'Stage interface test'
      }
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
