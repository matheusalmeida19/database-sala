# 📂 Database sala SQL

Este projeto é um **banco de dados SQL** criado para fins de estudo, baseado no que estou aprendendo na faculdade. Ele contém as tabelas **Customers, Orders e Shippings**, e pode ser executado localmente com SQLite.

---

## **Tecnologias Utilizadas**
- **SQLite** (Banco de Dados Relacional)
- **SQL** (Linguagem para manipulação de banco de dados)
- **VS Code** (Editor de Código)
- **Git/GitHub** (Versionamento)

---

## **Como Rodar o Projeto**
Siga os passos abaixo para configurar e rodar o banco de dados.

### **1️⃣ Instalar o SQLite**
Caso ainda não tenha o SQLite instalado, siga estes passos:

1. **Acesse o vídeo** [aqui]([https://www.sqlite.org/download.html](https://youtu.be/__cwh4oezac?si=NysaAppNZvlDgPLo)).
2. 
2️⃣ Clonar o Repositório
Abra o terminal (Git bash, CMD, PowerShell ou VS Code) e rode:

        git clone [https://github.com/matheusalmeida19/database-sala.git]
   
        cd database-sala
   
3️⃣ Criar o Banco de Dados
Execute os seguintes comandos:

    sqlite3 db/database.db
    
    .read src/tables.sql
    
Isso criará as tabelas e adicionará os dados ao banco.

Para verificar se tudo foi criado corretamente:

    .tables
    
    SELECT * FROM Customers;

    
4️⃣ Executar Consultas SQL
Para rodar as consultas SQL predefinidas, use:

    .read src/query.sql
Isso executará todas as consultas armazenadas no arquivo.

Se quiser rodar uma consulta manualmente, basta abrir o SQLite e digitar:

    SELECT * FROM Orders;
    
📝 Observações
Se der erro ao rodar .read src/tables.sql, tente usar o caminho completo:

    .read "C:/caminho-completo/src/tables.sql"
    
O arquivo database.db não está no repositório para evitar versionamento de dados. Se precisar, basta recriar o banco de dados com o script tables.sql.

🧑‍💻 Contribuição
Caso queira contribuir, siga os passos:

Faça um fork do projeto.
#
Crie um branch para sua alteração (git checkout -b minha-mudanca).
#
Faça o commit (git commit -m "Descrição da mudança").
#
Faça o push para seu branch (git push origin minha-mudanca).
#
Abra um Pull Request.
