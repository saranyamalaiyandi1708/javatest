pipeline {
  agent any

  tools {
    maven 'maven'
  }

  stages {
    stage('Build') {
        steps {
            sh 'mvn clean package'
        }
    }

    stage('Test') {
      steps {
          echo 'test...'
        }
    }


    stage('Code Quality') {
      steps {
          echo 'Quality'
        }
    }

    stage('Deploy to Dev') {
      steps {
          echo 'Dev'
        }
    }

    stage('Deploy to Test') {
      steps {
          echo 'Test'
        }
    }

    stage('Deploy to UAT') {
      steps {
          echo 'UAT'
        }
    }

    stage('Deploy to Pre_prod') {
      steps {
            echo 'Staging'
          }
    }

    stage('Prod Approval') {
      steps {
          echo 'Prod Approval'
               }
        
    }

    stage('Deploy to Prod') {
      when { branch 'master'}
      steps { 
          echo 'Prod'         
        }
    }
  }
