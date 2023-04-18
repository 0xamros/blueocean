pipeline {
  agent any
  stages {
    stage('buildld') {
      steps {
        echo 'Build compleated'
      }
    }

    stage('test') {
      parallel {
        stage('test2') {
          steps {
            echo 'running test2'
          }
        }

        stage('test1') {
          steps {
            echo 'test1 running'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment compleated'
      }
    }

  }
}