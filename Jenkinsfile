pipeline {
  agent any
  stages {
    stage('initialize') {
      parallel {
        stage('initialize') {
          steps {
            echo 'First Pipeline Message'
          }
        }

        stage('Test') {
          steps {
            fileExists 'ShoppingBasketTest.java'
          }
        }

      }
    }

  }
}