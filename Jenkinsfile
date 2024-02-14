pipeline {
  agent any
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf roles_grafana'
        sh 'git clone https://github.com/yatheesh2328/roles_grafana.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana_playbook.yml'
      }
    }
  }
}
