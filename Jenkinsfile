pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "Stage build"'
        sh 'cd $WORKSPACE && ls -al'
        sh '/usr/bin/gcc zombie.orphan.c -o zombie.out && chmod u+x zombie.out && ./zombie.out'
      }
    }

    stage('unitTest') {
      steps {
        echo 'Stage unit test'
      }
    }

  }
}
