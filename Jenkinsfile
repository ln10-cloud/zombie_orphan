pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "Stage build"'
        sh 'cd $WORKSPACE && ls -al'
        
      }
    }

    stage('unitTest') {
      steps {
        echo 'Stage unit test'
      }
    }

  }
}
