# Instalação do Kubernetes 🚀

Bem-vindo à seção de instalação do Kubernetes! Aqui, você encontrará instruções sobre como instalar o Kubernetes em seu ambiente.

## Kubernetes

O Kubernetes é uma plataforma de código aberto para automatizar a implantação, escalonamento e gerenciamento de aplicativos em contêiner. Siga as instruções abaixo para instalar o Kubernetes:

### 🐧 Linux

#### Minikube (Ambiente de Desenvolvimento Local)
1. Baixe o executável do Minikube: `curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64`.
2. Dê permissão de execução: `sudo chmod +x minikube-linux-amd64`.
3. Mova o executável para um diretório no seu caminho: `sudo mv minikube-linux-amd64 /usr/local/bin/minikube`.
4. Inicie o cluster: `minikube start`.

#### Kubectl (Cliente Kubernetes)
1. Baixe o executável do kubectl: `curl -LO https://dl.k8s.io/release/v1.22.0/bin/linux/amd64/kubectl`.
2. Dê permissão de execução: `sudo chmod +x kubectl`.
3. Mova o executável para um diretório no seu caminho: `sudo mv kubectl /usr/local/bin/kubectl`.
4. Verifique a instalação: `kubectl version --client`.

### 🪟 Windows

#### Minikube (Ambiente de Desenvolvimento Local)
1. Baixe o instalador do Minikube no site oficial: [Minikube Releases](https://github.com/kubernetes/minikube/releases).
2. Execute o instalador e siga as instruções para concluir a instalação.
3. Inicie o cluster: `minikube start`.

#### Kubectl (Cliente Kubernetes)
1. Baixe o executável do kubectl: [kubectl](https://dl.k8s.io/release/v1.22.0/bin/windows/amd64/kubectl.exe).
2. Adicione o diretório contendo o executável ao PATH do sistema.

### ℹ️ Nota
Certifique-se de revisar a documentação oficial do Kubernetes para obter informações mais detalhadas e atualizadas.

Lembre-se de que a instalação do Kubernetes pode variar dependendo do seu ambiente e dos requisitos específicos do seu projeto. Se precisar de mais alguma coisa, estou à disposição!
