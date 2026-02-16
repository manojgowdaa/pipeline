pipeline {
  agent any;
  stages {
    stage ('BUILD') {
      steps {
        echo "This is build stage"
      }
    }
    stage ('Test Parallel') {
      parallel {
        stage ('Test on CHROME') {
          steps {
            echo "This is testin in CHROME"
          } 
        }
        stage ('Test on OPERA') {
          steps {
            echo "This is testin in OPERA"
          } 
        }
      }
    }
    stage ('Deplooy') {
      steps {
        echo "This is deploy stage"
      }
    }
  }
}
#