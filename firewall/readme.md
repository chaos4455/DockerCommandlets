# Firewall UFW 🚧

Bem-vindo ao repositório de Firewall UFW! Aqui, você encontrará informações e scripts relacionados ao Uncomplicated Firewall (UFW), uma ferramenta para gerenciar o firewall no Linux. 🔒

## O que é o UFW?

O UFW, ou Uncomplicated Firewall, é uma interface de linha de comando para o iptables e destina-se a simplificar o processo de gerenciamento de firewalls no Linux.
# Firewall UFW 🛡️

Bem-vindo ao tutorial de Firewall UFW para Docker! Neste guia, você aprenderá a configurar o Uncomplicated Firewall (UFW) no Linux para garantir uma camada adicional de segurança ao trabalhar com o Docker. 🚀

## Introdução

O UFW é uma ferramenta de firewall fácil de usar para gerenciar regras de filtragem no Linux. Vamos integrá-lo ao Docker para controlar o tráfego de rede.

## Configuração Básica do UFW

1. **Instalação do UFW:**
   - Certifique-se de ter o UFW instalado em seu sistema.
     ```bash
     sudo apt-get update
     sudo apt-get install ufw
     ```

2. **Definindo Políticas Padrão:**
   - Configure as políticas padrão para permitir o tráfego de saída e bloquear o tráfego de entrada.
     ```bash
     sudo ufw default allow outgoing
     sudo ufw default deny incoming
     ```

3. **Permitindo Portas do Docker:**
   - Abra as portas necessárias para o Docker (por exemplo, 80 para HTTP).
     ```bash
     sudo ufw allow 80/tcp
     ```

## Integração com o Docker

1. **Habilitando o UFW:**
   - Ative o UFW.
     ```bash
     sudo ufw enable
     ```

2. **Permitindo o Tráfego Docker:**
   - Adicione regras para permitir o tráfego Docker.
     ```bash
     sudo ufw allow 2375/tcp     # Docker API
     sudo ufw allow 2376/tcp     # Docker TLS
     ```

3. **Reiniciando o Docker e o UFW:**
   - Reinicie o Docker e o UFW para aplicar as alterações.
     ```bash
     sudo systemctl restart docker
     sudo systemctl restart ufw
     ```

## Testando a Configuração

Certifique-se de testar a configuração acessando o Docker de maneira segura e verificando se as regras do UFW estão sendo aplicadas corretamente.

## Contribuição

Sinta-se à vontade para contribuir! Adicione melhorias ao tutorial, novas dicas ou informações adicionais sobre o UFW. Contribuições são sempre bem-vindas! 🎉


## Contribuição

Sinta-se à vontade para contribuir! Adicione novas regras, tutoriais ou melhore a documentação existente. Contribuições são sempre bem-vindas! 🎉
