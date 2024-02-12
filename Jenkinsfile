pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf grafana-repo'
        sh 'git clone https://github.com/sudhasanshi/grafana-repo.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana1.yml'
      }
    }
  }
}
