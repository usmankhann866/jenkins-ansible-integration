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
        ansiblePlaybook(playbook: 'ansible/playbooks/setup.yml', inventory: 'ansible/inventory/hosts', limit: 'localhost')


}
    }

  }

}
