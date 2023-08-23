node {
  stage('SCM') {
    checkout scm
  }

  stage('SonarQube Analysis') {
    def scannerHome = tool 'S3';
    withSonarQubeEnv() {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }

  stage("Running npm build"){
    echo "npm buil"
  }

  stage("Running npm test"){
    echo "npm test"
  }
}
