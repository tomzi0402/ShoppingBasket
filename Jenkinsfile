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
            fileExists 'src/test/ShoppingBasketTest1.java'
            readFile(encoding: 'UTF-8', file: 'src/test/Item.java')
          }
        }

      }
    }

  }
}