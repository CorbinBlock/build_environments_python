pipeline {
    agent none
    stages {         
        stage('WIN-01-LENOVO') {
            agent {
                label 'WIN-01-LENOVO'
            }
            steps {
                pwsh("""
                python update_nodes.py
                """)
            }
        }
        stage('WIN-02-ASUS') {
            agent {
                label 'WIN-02-ASUS'
            }
            steps {
                pwsh("""
                python update_nodes.py
                """)
            }
        }
        stage('UNIX-01-DEBIAN') {
            agent {
                label 'UNIX-01-DEBIAN'
            }
            steps {
                sh"""
                python3 update_nodes.py                
                """
            }
        }
        stage('UNIX-02-FEDORA') {
            agent {
                label 'UNIX-02-FEDORA'
            }
            steps {
                sh"""
                python update_nodes.py
                """
            }
        }
    }
}