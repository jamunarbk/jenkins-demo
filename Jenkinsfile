pipeline{
  agent any
  stages{
    stage('Checkout Code'){
      steps{
        git 'https://github.com/jamunarbk/jenkins-demo.git'
      }
    }
    stage ('Build'){
      steps{
        echo "Building application..."
      }
    }
    stage('Test'){
      steps{
        echo "Running tests..."
      }
    }
  }
  post{
    success{
      echo "Pipeline executed from SCM successfully!"
    }
    failure{
      echo "Pipeline failed. Fix code and retry."
    }
  }
}
