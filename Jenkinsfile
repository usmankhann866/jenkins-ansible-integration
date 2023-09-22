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
        ansiblePlaybook(playbook: 'ansible/java-app-setup.yml', inventory: 'ansible/hosts', limit: 'localhost', vaultCredentialsId: "java-app-vault")


}
    }

  }

