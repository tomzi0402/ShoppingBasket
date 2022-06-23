pipeline {
  agent any
  stages {
    stage('initialize') {
      parallel {
        stage('Print Message') {
          steps {
            echo 'First Pipeline Message'
          }
        }

        stage('Test File Exists') {
          steps {
            fileExists 'ShoppingBasketTest1.java'
          }
        }

      }
    }

  }
}