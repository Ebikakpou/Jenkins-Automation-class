
pipeline {
    agent any

    stages {
      stage('Build & Test') {
    steps {
        sh 'python3 -m pip install pytest'
        sh 'python3 -m pytest test_backup.py'
    }
}

        stage('Deploy') {
            steps {
                sh 'python3 run_all.py'
            }
        }
    }
}
