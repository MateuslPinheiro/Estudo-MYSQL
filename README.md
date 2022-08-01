## Estudo-MYSQL
Repositório contendo anotações de meus estudos em MYSQL.


![image](https://user-images.githubusercontent.com/102734845/175659426-1944d382-335f-4009-ba2c-4e2e84b4cb87.png)

## Configuração de Ambiente:
Como instalar o MySQL 8.0 no Ubuntu Linux
Siga os passos abaixo para realizar a instalação do MySQL 8 e do MySQL Workbench
no Ubuntu Linux.

1. Baixar o pacote do repositório apt do MySQL:
```
$ wget -c https://repo.mysql.com//mysql-apt-config_0.8.23-1_all.deb
```
Para saber qual a versão do repositório baixar, acessar a página:
```
https://dev.mysql.com/downloads/repo/apt/
```

2. Instalar o pacote do repositório:
```
$ sudo dpkg -i mysql-apt-config_0.8.23-1_all.deb
```
3. Instalar o MySQL Server:
```
$ sudo apt update
$ sudo apt install mysql-server
```
4. Rodar script para configurar instalação segura:
```
$ sudo mysql_secure_installation
```
### Perguntas:
Senha para validar componente? ```Enter``` (N)

Mudar senha do root? ```Enter``` (N)

Remover usuários anônimos? ```Y```

Desabilitar login de root remoto? ```Y```

Remover banco de dados de teste? ```Y```

Recarregar tabelas de privilégio? ```Y```

5. Verificar status do serviço:
```
$ sudo systemctl status mysql
```
Pressione ```Q``` Para sair

6. Iniciar serviço, se necessário:
```
$ sudo systemctl start mysql
```
7. Habilitar inicialização automática do MySQL Server:
```
$ sudo systemctl enable mysql
```
8. Instalar MySQL Workbench:
```
$ sudo apt install mysql-workbench-community
```
9. Acessar pelo terminal para testar:
```
$ sudo mysql -u root -p
```
10. Abrir MySQL Workbench para testar, via interface gráfica.
