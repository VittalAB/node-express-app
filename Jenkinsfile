pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch : "main",
                    url : "https://github.com/VittalAB/node-express-app.git"
            }
        }

      stage("npm build"){
        steps{

          echo "npm build is going on"
        }
    }

      stage("npm test"){
        steps{
            echo "npm test is going on"
      }  
    }
}
