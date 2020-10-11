pipeline {
  agent any
  stages {
    stage('job1') {
      parallel {
        stage('job1') {
          steps {
            build 'demo'
          }
        }

        stage('job2') {
          steps {
            build 'job3'
          }
        }

      }
    }

    stage('') {
      steps {
        build 'job2'
      }
    }

  }
}