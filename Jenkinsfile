pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Faz checkout do código do repositório Git configurado no job
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Apenas imprime uma mensagem para simular build
                echo 'Executando build simples...'
                // Comando simples para testar, pode ser substituído pelo build real
                sh 'echo Hello, Jenkins Pipeline!'
            }
        }
        stage('Test') {
            steps {
                echo 'Executando testes simulados...'
                // Simula teste com comando simples
                sh 'echo Testes OK!'
            }
        }
    }
    post {
        always {
            echo 'Pipeline finalizado.'
        }
    }
}
