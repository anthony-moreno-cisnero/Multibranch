pipeline {

  agent any

  stages {

    stage("App Versions"){  
      steps {
        script{
          sh "npm -version"
          sh "node -v"
        }
      }
    }
    stage("User ID"){  
      steps {
        script{
          sh "id"
        }
      }
    }
  }
  post {
    always {          
      deleteDir()
      sh "echo 'always'"
    }

    success {
      sh "echo 'success'"
    }

    failure {
      sh "echo 'failure'"
    }  
  }
} 

