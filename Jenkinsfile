pipeline {

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
