pipeline {

  environment {
    registry = "localhost:5000/justme/myweb1"
    dockerImage = ""
  }

  agent any

  stages {
    stage('Deploy The App') {
      steps {
        script {
          kubernetes.deploy(configs: "client-cluster-ip-service.yaml", kubeconfigId: "mykubeconfiguration")
        }
      }
    }

  }

}
