pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "Stage build"'
        sh 'echo Build_ID : ${env.BUILD_ID}'
        sh 'echo Build_Number: ${env.BUILD_NUMBER}'
        sh 'cd $WORKSPACE && ls -al'
        /*
        sh 'gcc zombie.orphan.c -o zombie.out && chmod u+x zombie.out && ./zombie.out'
        */
      }
    }

    stage('unitTest') {
      steps {
        echo 'Stage unit test'
      }
    }

  }
}
