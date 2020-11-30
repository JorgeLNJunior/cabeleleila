<div align="center">
   <h1>Cabeleleila</h1>
   <p>App para gestão de reservas de salões de beleza para a matéria de programação mobile.</p>
</div>

## Requerimentos
- Uma conta na plataforma [Monaca](https://monaca.io/)
- Uma conta na plataforma [Firebase](http://firebase.com/)

## Instalação
- Monaca
    - Crie um novo projeto em branco
    - Copie todos os arquivos HTML para o projeto monaca (contas PRO podem importar projetos a partir de urls do GitHub)

- Firebase
    - Crie um novo projeto no firebase
    - Registre um novo aplicativo web
    - Adicione as credenciais em todas as páginas HTML no monaca
    - Em `Authentication` habilite a autenticação por email e senha
    - Em `Realtime Database` crie um novo banco de dados com as seguites regras:
    ```
    {  
        "rules": {  
            ".read": true,
            ".write": "auth != null",
        }
    }   
    ```

## Critéios da aplicação

- [x] Interface amigável
- [x] Salvar e ler informções na base SQLite
- [x] Ter conexão com Firebase, efetuando as operações de CRUD (Create,
Read, Update e Delete)
