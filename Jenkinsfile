pipeline {
    agent none
    stages {         
        stage('WIN-01-LENOVO') {
            agent {
                label 'WIN-01-LENOVO'
            }
            steps {
                pwsh("""
                cd python/os
                python3 subprocess_run.py
                """)
            }
        }
        stage('WIN-02-ASUS') {
            agent {
                label 'WIN-02-ASUS'
            }
            steps {
                pwsh("""
                cd python/os
                python3 subprocess_run.py
                """)
            }
        }
        stage('UNIX-01-DEBIAN') {
            agent {
                label 'UNIX-01-DEBIAN'
            }
            steps {
                sh"""
                cd python/os
                python3 subprocess_run.py
                
                """
            }
        }
        stage('UNIX-02-FEDORA') {
            agent {
                label 'UNIX-02-FEDORA'
            }
            steps {
                sh"""
                cd python/os
                python3 subprocess_run.py
                """
            }
        }
    }
}