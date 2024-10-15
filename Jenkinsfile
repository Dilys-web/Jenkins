pipeline{
  agent any
  stage ("Run application"){
    steps{
      script{ 
        sh "python3 new.py"
      }
    }
  }
  post{
    always{
      cleanWs()
    }
    success{
      script{
        echo "Successful"
  
      }
    }
    failure{
      script {
        echo "Failure"
    }
    
  }
}
