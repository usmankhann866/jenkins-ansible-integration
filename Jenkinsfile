pipeline {
  agent {
    node {
      label 'linux'
    }

  }
  stages {
    stage('Build') {
      steps {
	echo "Hello world"
      }
    }

    stage('Test') {
      steps {
       
       ansiblePlaybook credentialsId: '5f591e89-ae17-4790-a0b7-f3db2d4d407f', disableHostKeyChecking: true, installation: 'Ansible', inventory: '/ansible/inventory/hosts', playbook: '/ansible/playbooks/setup.yml'

}
    }

  }

}
