pipeline {
    agent any 
    stages {
         stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo 'Construyendo la Aplicación' 
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
        stage('Test') { 
            steps {
                echo 'Arranca el proceso de pruebas unitarias' 
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Desplegando al área de desarrollo' 
            }
        }
    }
}
