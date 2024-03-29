# Hotel Econômico
Gerenciador de hospedagens para pousada/pensão. Comecei a desenvolver aplicação em 2016 para uma pensão onde eu morava, mas logo ela foi vendida para outra pessoa.

# Imagem
![image](https://user-images.githubusercontent.com/15344931/122095274-8a825680-cde3-11eb-97dd-c4999478b133.png)


# Criando e populando banco de dados
Script para criar banco (Transact-SQL)
https://github.com/ezxpro/Hotel-Economico/blob/main/CriaBanco.sql

É necessário modificar o script para alterar os caminhos onde serão armazenados os arquivos do banco de dados.

# Requisitos
1. Visual Studio 2016/2019
2. .NET 4.6.1
3. SQL Server Express/LocalDB Express 2016
4. SQL Server Management Studio 2018 (SMSS)

No caso do SQL Server LocalDB, para que o programa se conecte do banco de dados é preciso iniciar a instância (por padrão a instância se chama MSSQLLocalDB) do banco de dados através do comando `SQLLocalDB start MSSQLLocalDB`. 

Após instalado SMSS e LocalDB, e a instância deste último iniciada, é necessário criar o banco usando o arquivo `CriaBanco.sql`. Para conectar à instância do localDB, deve ser passada a seguinte string de conexão no smss: 
```
(localdb)\MSSQLLocalDB
```
Usando o modo de autenticação `autenticação do Windows`, a conexão deve ser estabelecida automaticamente. Em seguida, deve-se executar o script SQL mencionado acima