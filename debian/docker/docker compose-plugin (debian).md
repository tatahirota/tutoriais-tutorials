#**INSTALAÇÃO DO DOCKER + PLUGIN COMPOSE  // DOCKER INSTALLATION + COMPOSE PLUGIN**<br>

1- BAIXAR O DOCKER // DOWNLOAD DOCKER: <br>
  sudo apt install apt-transport-https ca-certificates curl gnupg2 software-properties-common
  ![image](https://github.com/user-attachments/assets/91abea22-da14-4dbb-991c-fda57b357ea2)

EXPLICAÇÃO // EXPLANATION: <br>
•  apt-transport-https: Esse pacote permite que o APT (o gerenciador de pacotes do Debian) consiga baixar pacotes usando o protocolo HTTPS, o que é essencial para repositórios seguros.<br>
                        This package allows APT (Debian's package manager) to download packages using the HTTPS protocol, which is essential for secure repositories.<br>
•  ca-certificates: Esse pacote instala certificados de autoridade confiáveis (CA). Ele é necessário para validar as conexões seguras HTTPS.<br>
                    This package installs trusted authority (CA) certificates. It is required to validate secure HTTPS connections. <br>
•  curl: Ferramenta de linha de comando para transferir dados com URLs. É usado para baixar o script de instalação do Docker.<br>
         Command line tool for transferring data with URLs. It is used to download the Docker installation script.<br>
•  gnupg2: Pacote para gerenciar chaves GPG, usado para verificar assinaturas e autenticidade dos pacotes.<br>
•  software-properties-common: Esse pacote contém ferramentas para gerenciar repositórios de pacotes, como adicionar e remover repositórios.<br>
