pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        build 'PES2UG21CS251-1'
        sh 'g++ main.cpp -o output'

      }
    }
    stage('Test'){
      steps{
      sh './ou'
      }
    }
    stage('Deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
}
}
