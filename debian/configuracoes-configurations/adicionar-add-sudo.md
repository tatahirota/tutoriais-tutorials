# SUDO PARA UM USUÁRIO COMUM   
# SUDO FOR A REGULAR USER   
  
_________________________________________________________________________________________________________________________   
 
## 1- Verifique o grupo.   
## 1- Check the group.   

![image](https://github.com/user-attachments/assets/3a098c68-106e-49d2-bec0-ce5b365152e2)    

O usuário está no grupo "users".   
The user is in the "users" group.    
   
<br>   

_________________________________________________________________________________________________________________________   

## 2- Usar o comando “su –“ e colocar a senha para entrar como “root”.   
## 2- Use the “su –“ command and enter the password to log in as “root”.    

![image](https://github.com/user-attachments/assets/9cf6a635-8836-4152-aecb-2353e313cf89)    

<br>    

_________________________________________________________________________________________________________________________  

## 3- Adicionar o Usuário ao grupo sudo.    
## 3- Add user to sudo group.   
****= nome de usuário   
****= username   
![image](https://github.com/user-attachments/assets/a6744e98-e09a-418a-a7f2-75629370612a)   

<br>    

_________________________________________________________________________________________________________________________

## 4- Verificar o grupo do usuário adicionado ao grupo “sudo”.   
## 4- Check the group of the user added to the “sudo” group.   
    
![image](https://github.com/user-attachments/assets/c8c7218c-8673-4208-b7ad-176f7e2b3625)    

O usuário agora está no grupo "sudo".   
The user is now in the "sudo" group.   

<br>    

_________________________________________________________________________________________________________________________

## 5- Vamos sair do “root” e ir para nosso usuário, e verificar o grupo sudo.   
## 5- Let’s exit “root” and go to our user, and check the sudo group.   

 ![image](https://github.com/user-attachments/assets/6d957647-575a-47dc-adba-cc35d2b28678)   

  sudo: nome do grupo
x: indica que a senha do grupo, se houver, está armazenada no arquivo “/etc/gshadow”.
27: GID (Group ID) do grupo “sudo”.
****: onde está censurado é o nome do usuário, indicando que no grupo sudo, o nosso usuário é um deles.   

sudo: group name
x: indicates that the group password, if any, is stored in the file “/etc/gshadow”.
27: GID (Group ID) of the “sudo” group.
****: where it is censored is the user name, indicating that in the sudo group, our user is one of them.   

<br>    

_________________________________________________________________________________________________________________________   

## 6- Para atualizar o grupo, coloque o comando a seguir.   
## 6- To update the group, enter the following command.   

![image](https://github.com/user-attachments/assets/4937f5dd-c881-422c-81de-4690e60eef6a)    

Pronto! :)  
Done! :)    

<br>   

 _________________________________________________________________________________________________________________________   




   
 

 
