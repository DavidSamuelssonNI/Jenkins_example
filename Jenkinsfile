pipeline {
    agent {
        node {
            label 'my_node'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                archiveArtifacts artifacts: 'AddTwoNumbers.vi', followSymlinks: false
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
