pipeline{
  agent any
  stages{
    stage('Preparation'){
      steps{
        git branch: 'main',
        url: 'https://github.com/nivigh/jenkinassign4.git',
        credentialsId:'github'
        sh 'javac first.java'
        sh 'java first'
      }
    }
        stage('Build'){
        steps {
            echo 'build started'
            sleep 2
            echo 'Build Completed'
        }
    }
    stage('Test'){
        steps {
            echo 'Test started'
            sleep 2
            echo 'Test Completed'
        }
    }
  }
}
