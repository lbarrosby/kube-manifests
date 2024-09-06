pipeline {
    agent any  // Usa qualquer agente disponível para executar o pipeline

    stages {
        stage('Preparação') {
            steps {
                // Certifique-se de que você tem o código necessário no workspace
                checkout scm  // Faz o checkout do código do repositório
            }
        }
        
        stage('Aplicar Configuração Istio') {
            steps {
                script {
                    // Muda para o diretório istio
                    dir('istio') {
                        // Aplica a configuração do Istio
                        sh 'ls -la'
                    }
                }
            }
        }
    }
}

