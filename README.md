# Fiap.Web.Alunos

Fiap.Web.Alunos é uma aplicação web desenvolvida com ASP.NET Core MVC, destinada à gestão de clientes, pedidos, produtos e lojas. Este projeto acadêmico simula funcionalidades de um sistema de controle comercial, usando boas práticas de desenvolvimento web, como padrão MVC, injeção de dependência e persistência com Entity Framework.

## 📦 Tecnologias Utilizadas

- ASP.NET Core MVC
- C#
- Razor (Views com .cshtml)
- Entity Framework Core (ORM)
- SQL Server (padrão, configurável)
- Docker (Dockerfile incluso)
- Bootstrap (nas views)
- Visual Studio ou VS Code

## 📁 Estrutura do Projeto

Fiap.Web.Alunos/
├── Controllers/
│   ├── HomeController.cs
│   └── ClienteController.cs
├── Models/
│   ├── ClienteModel.cs
│   ├── PedidoModel.cs
│   ├── PedidoProdutoModel.cs
│   ├── LojaModel.cs
│   └── Fornecedor.cs
├── Data/
│   └── Contexts/DatabaseContext.cs
├── Views/
│   ├── Cliente/ (Index, Create, Cadastro)
│   ├── Home/ (Index, Privacy)
│   └── Shared/ (_Layout, Error, etc.)
├── Program.cs
├── appsettings.json
├── Dockerfile
└── Fiap.Web.Alunos.csproj

## ✅ Funcionalidades

- Cadastro e listagem de clientes
- Cadastro de pedidos e produtos associados
- Interface web com páginas Razor
- Layout base e partials compartilhados
- Validação de formulários
- Integração com banco de dados relacional

## ⚙️ Como Executar

### Requisitos

- .NET SDK 6.0 ou superior
- SQL Server LocalDB ou instância padrão
- Visual Studio 2022+ ou Visual Studio Code
- Docker (opcional)

### Passos

1. **Clone o repositório:**
   git clone https://github.com/LeItaloWork/Fiap.Web.Alunos.git

2. **Restaure os pacotes:**
   dotnet restore

3. **Configure a string de conexão em:**
   `appsettings.json`

4. **Execute as migrations (se houver):**
   dotnet ef database update

5. **Inicie a aplicação:**
   dotnet run

6. **Acesse no navegador:**
   http://localhost:5000 ou https://localhost:5001

## 🐳 Docker (Opcional)

1. Build da imagem:
   docker build -t fiapwebalunos .

2. Execute o container:
   docker run -d -p 8080:80 fiapwebalunos

Acesse: http://localhost:8080

