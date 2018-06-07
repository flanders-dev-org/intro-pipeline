pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello ') {
      steps {
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        echo "Hello ${MY_NAME }"
        sh 'java -version'
      }
    }
  }
  environment {
    TEST_USER = credentials('test-user')
    MY_NAME = 'Mary'
  }
}