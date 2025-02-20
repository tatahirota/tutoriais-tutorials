# INSTALAÇÃO DO DOCKER + PLUGIN COMPOSE  // DOCKER INSTALLATION + COMPOSE PLUGIN**<br>
   
## 1- BAIXAR O DOCKER // DOWNLOAD DOCKER: <br>
  sudo apt install apt-transport-https ca-certificates curl gnupg2 software-properties-common   

<br>   


![image](https://github.com/user-attachments/assets/4a7a6a5d-97b1-418f-bc87-a76fb42859c6)    

<br>   
   
   
EXPLICAÇÃO // EXPLANATION: <br>
• apt-transport-https: Esse pacote permite que o APT (o gerenciador de pacotes do Debian) consiga baixar pacotes usando o protocolo HTTPS, o que é essencial para repositórios seguros.    
• apt-transport-https: This package allows APT (Debian's package manager) to download packages using the HTTPS protocol, which is essential for secure repositories.   

<br>   
   
• ca-certificates: Esse pacote instala certificados de autoridade confiáveis (CA). Ele é necessário para validar as conexões seguras HTTPS.   
• ca-certificates: This package installs trusted authority (CA) certificates. It is needed to validate secure HTTPS connections.   

<br>   

• curl: Ferramenta de linha de comando para transferir dados com URLs. É usado para baixar o script de instalação do Docker.   
• curl: A command-line tool for transferring data with URLs. It is used to download the Docker installation script.   

<br>   
   
• gnupg2: Pacote para gerenciar chaves GPG, usado para verificar assinaturas e autenticidade dos pacotes.   
• gnupg2: A package for managing GPG keys, used to verify package signatures and authenticity.   

<br>   

• software-properties-common: Esse pacote contém ferramentas para gerenciar repositórios de pacotes, como adicionar e remover repositórios.   
• software-properties-common: This package contains tools for managing package repositories, such as adding and removing repositories.   

<br>   
      
----------------------------------------------------------------------------------------------------------------   

<br>   

## 2-BAIXAR E ARMAZENAR A CHAVE GPG CORRETAMENTE PARA USO NO APT. A chave GPG é usada para assinar digitalmente pacotes de software e garantir que eles não foram modificados por terceiros antes de serem instalados, e no docker, essa chave do repositório oficial serve para validar que os pacotes que você baixa são legítimos e não foram adulterados.
## 2-DOWNLOAD AND  STORE THE GPG KEY  CORRECTLY FOR USE IN APT. The GPG key is used to digitally sign software packages and ensure that they have not been modified by third parties before being installed, and in docker, this key from the official repository serves to validate that the packages you download are legitimate and have not been tampered with.

curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg   
   
<br>        
   
![image](https://github.com/user-attachments/assets/dca1c5f4-75cf-468a-bb87-cbd93e38de0a)  
    
<br>  
   
EXPLICAÇÃO /// EXPLANATION:   
   
• curl -fsSL https://download.docker.com/linux/debian/gpg. Esse trecho usa o curl para baixar a chave GPG do repositório oficial do Docker.      
• curl -fsSL https://download.docker.com/linux/debian/gpg. This snippet uses curl to download the GPG key from the official Docker repository.   
   
 curl → Comando para fazer requisições HTTP e baixar arquivos.   
 curl → Command to make HTTP requests and download files.   
    
-f (fail silently) → Se houver erro, não exibe mensagens de erro na saída padrão.   
-f (fail silently) → If there is an error, do not display error messages on standard output.   
   
-s (silent) → Oculta a barra de progresso.   
-s (silent) → Hide the progress bar.   
   
-S (show errors) → Se houver erro, mostra apenas a mensagem de erro.   
-S (show errors) → If there is an error, only show the error message.   
   
-L (follow redirects) → Se o link redirecionar para outro, o curl seguirá esse redirecionamento.   
-L (follow redirects) → If the link redirects to another link, curl will follow that redirection.   
   
📌 Resumo: Esse trecho baixa a chave GPG do Docker.   
📌 Summary: This snippet downloads the Docker GPG key.   
   
 <br>   
   
• | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg .Esse trecho usa o GPG para armazenar a chave de forma segura.   
• | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg .This snippet uses GPG to store the key securely.   

• | → O pipe (|) envia a saída do curl como entrada para o próximo comando (gpg).   
• | → The pipe (|) sends the output of curl as input to the next command (gpg).   

• sudo → Executa como root (necessário para salvar no diretório /usr/share/keyrings/).   
• sudo → Run as root (required to save in the /usr/share/keyrings/ directory).   
   
• gpg → Comando do GNU Privacy Guard, que gerencia chaves GPG.   
• gpg → GNU Privacy Guard command, which manages GPG keys.   

• --dearmor → Converte a chave para um formato binário adequado para uso pelo APT.   
• --dearmor → Converts the key to a binary format suitable for use by APT.   

• -o /usr/share/keyrings/docker-archive-keyring.gpg  
      -o → Define um arquivo de saída.    
      /usr/share/keyrings/docker-archive-keyring.gpg → Local onde a chave será salva.   
• -o /usr/share/keyrings/docker-archive-keyring.gpg  
      -o → Specifies an output file.   
      /usr/share/keyrings/docker-archive-keyring.gpg → Location where the key will be saved.   

📌 Resumo: Esse trecho converte a chave para um formato adequado e a salva no diretório seguro.   
📌 Summary: This snippet converts the key to a suitable format and saves it in the secure directory.   

<br>   
   
-----------------------------------------------------------------------------------------------------------   

<br>   






