# Instalação do Docker e Docker Machine 🐳

Bem-vindo à seção de instalação do Docker e Docker Machine! Aqui, você encontrará instruções sobre como instalar o Docker em sistemas Debian/Ubuntu e o Docker Machine no Windows.

## Instalação do Docker no Debian/Ubuntu

### 🐧 Debian
1. Atualize o índice de pacotes: `sudo apt-get update`.
2. Instale pacotes para permitir o apt usar um repositório sobre HTTPS: `sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release`.
3. Adicione a chave GPG oficial do Docker: `curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`.
4. Adicione o repositório Docker ao sources.list.d: `echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/debian $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null`.
5. Atualize o índice de pacotes novamente: `sudo apt-get update`.
6. Instale a versão mais recente do Docker: `sudo apt-get install docker-ce docker-ce-cli containerd.io`.

### 🐧 Ubuntu
1. Atualize o índice de pacotes: `sudo apt-get update`.
2. Instale pacotes para permitir o apt usar um repositório sobre HTTPS: `sudo apt-get install apt-transport-https ca-certificates curl software-properties-common`.
3. Adicione a chave GPG oficial do Docker: `curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`.
4. Adicione o repositório Docker ao sistema: `sudo add-apt-repository "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"`.
5. Atualize o índice de pacotes novamente: `sudo apt-get update`.
6. Instale a versão mais recente do Docker: `sudo apt-get install docker-ce docker-ce-cli containerd.io`.

## Instalação do Docker Machine no Windows

1. Baixe o instalador do Docker Machine para Windows: [Docker Machine Release](https://github.com/docker/machine/releases).
2. Execute o instalador e siga as instruções para concluir a instalação.
3. Verifique a instalação executando o comando no PowerShell: `docker-machine version`.

Lembre-se de conferir a documentação oficial para obter informações mais detalhadas e atualizadas.

