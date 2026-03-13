# CSMSage - Advanced API & Licensing System

O **CSMSage** é uma solução empresarial concebida para fornecer uma camada de API Rest robusta sobre o software **Sage 50c**, acompanhada por um painel de controlo administrativo para gestão de licenciamento e segurança.

## 🚀 Estrutura do Projeto

O ecossistema é composto por dois módulos principais:

### 1. CSMSage Engine (Servidor .NET)
Localizado na pasta `CSMSage/`, é o núcleo do sistema.
- **Tecnologia**: .NET 8.0, ASP.NET Core API.
- **Função**: Expõe os dados do Sage 50c (Clientes, Documentos, Stocks) via JSON.
- **Segurança**: Protegido por um Middleware de API Key que valida pedidos contra o servidor de licenciamento.
- **Documentação**: OpenAPI/Swagger integrada e documentação interativa via Scalar.

### 2. Painel de Licenciamento (Web Portal)
Localizado na pasta `license_panel/`.
- **Tecnologia**: PHP (Vanilla), MySQL/MariaDB, Bootstrap 5.
- **Função**: Portal administrativo para:
    - Geração de chaves de API (Licenças).
    - Gestão de clientes e organizações.
    - Monitorização de utilização (Last Used).
    - Página de registo público para o Programa Beta.
- **Design**: Estética SaaS moderna, focado na experiência de utilização e rapidez.

## 🛠️ Requisitos e Instalação

### Engine .NET
1. Certifique-se de ter o **SDK .NET 8.0** instalado.
2. Configure o ficheiro `appsettings.json` com os detalhes da base de dados do Sage 50c.
3. Execute o comando:
   ```bash
   dotnet watch run
   ```

### Painel PHP
1. Requer um servidor web (Apache/Nginx) com **PHP 7.4+**.
2. SQL: Importe a estrutura da base de dados (tabela `licenses` e `users`).
3. Configure os detalhes de ligação em `config/database.php`.

## 📦 Funcionalidades Principais
- [x] **API Rest para Sage 50c**: Leitura e escrita de documentos de faturação.
- [x] **Gestão de Licenças**: Controlo total sobre quem pode aceder à API.
- [x] **Cópia Rápida**: Botões inteligentes para copiar chaves de acesso.
- [x] **Programa Beta**: Automatização da entrada de novos parceiros.
- [x] **Segurança Centralizada**: Validação em tempo real entre o PHP e o C#.

## 📝 Notas de Versão (Beta)
*   **Limites de Utilização**: O sistema já transporta limites de utilizadores, com implementação de bloqueio planeada para versões futuras.
*   **Documentação**: Aceda a `/api/docs` para visualizar o catálogo completo de rotas disponíveis.

---
© 2026 CSMSage Advanced Licensing | Desenvolvido para máxima performance com Sage 50c.
