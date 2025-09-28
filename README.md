# CSMSage API - Sistema de Gestão Comercial

<div align="center">

![CSMSage Logo](https://img.shields.io/badge/CSMSage-API-blue?style=for-the-badge&logo=api)
![Version](https://img.shields.io/badge/version-1.0.0-green?style=for-the-badge)
![License](https://img.shields.io/badge/license-Proprietary-red?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-Windows-blue?style=for-the-badge&logo=windows)

**Sistema completo de gestão comercial com API REST integrada**

[🚀 Obter Chave API Beta](#-obter-chave-api-beta) • [📖 Documentação](#-documentação) • [🛠️ Instalação](#️-instalação) • [⚙️ Configuração](#️-configuração)

</div>

---

## 📋 Índice

- [🎯 Sobre o Projeto](#-sobre-o-projeto)
- [✨ Funcionalidades](#-funcionalidades)
- [🚀 Obter Chave API Beta](#-obter-chave-api-beta)
- [🛠️ Instalação](#️-instalação)
- [⚙️ Configuração](#️-configuração)
- [📖 Documentação da API](#-documentação-da-api)
- [🔧 Desenvolvimento](#-desenvolvimento)
- [📞 Suporte](#-suporte)

---

## 🎯 Sobre o Projeto

O **CSMSage API** é um sistema completo de gestão comercial desenvolvido em C# .NET que oferece uma API REST robusta para integração com sistemas externos. O sistema inclui gestão de clientes, produtos, transações de stock, documentos comerciais e muito mais.

### 🏗️ Arquitetura

- **Backend**: C# .NET 8.0 com ASP.NET Web API
- **Frontend**: Windows Forms com interface moderna
- **Base de Dados**: SQL Server integrado
- **Autenticação**: Sistema de licenças com validação online
- **API**: RESTful com documentação Swagger integrada

---

## ✨ Funcionalidades

### 🏢 Gestão Comercial
- ✅ **Clientes**: CRUD completo com pesquisa avançada
- ✅ **Fornecedores**: Gestão de fornecedores e contactos
- ✅ **Produtos**: Catálogo de produtos com gestão de stock
- ✅ **Unidades de Medida**: Sistema flexível de unidades

### 📊 Transações e Movimentos
- ✅ **Transações de Stock**: Entradas, saídas e ajustes
- ✅ **Transações de Conta**: Movimentos financeiros
- ✅ **Documentos**: Gestão de documentos comerciais
- ✅ **Relatórios**: Sistema de relatórios integrado

### 🔌 API REST
- ✅ **Endpoints Completos**: Todos os módulos disponíveis via API
- ✅ **Autenticação**: Sistema seguro de chaves API
- ✅ **Documentação**: Swagger UI integrado
- ✅ **Validação**: Validação robusta de dados

### 🔐 Sistema de Licenças
- ✅ **Validação Online**: Verificação automática de licenças
- ✅ **Gestão Centralizada**: Painel administrativo web
- ✅ **Licenças Beta**: Acesso gratuito durante fase beta
- ✅ **Segurança**: Encriptação e proteção de dados

---

## 🚀 Obter Chave API Beta

### 🎁 Programa Beta Gratuito

Durante a fase beta, oferecemos **chaves API completamente gratuitas** com acesso ilimitado a todas as funcionalidades.

### 📝 Como Obter a Sua Chave

1. **Aceda ao Portal Beta**: [https://50capi.csmanager.ovh/beta_signup.php](https://50capi.csmanager.ovh/beta_signup.php)

2. **Preencha o Formulário**:
   - Nome completo
   - Email válido
   - Nome da empresa (opcional)

3. **Receba a Sua Chave**:
   - Chave API gerada automaticamente
   - Licença ilimitada (sem data de expiração)
   - Acesso a todas as funcionalidades

### 🔑 Exemplo de Chave API
```
997E856A-E3C37B15-5AAEF78D-091B0CAF
```

### 📋 Instruções de Uso
Após obter a sua chave, consulte as [Instruções Detalhadas](https://50capi.csmanager.ovh/beta_instructions.php) para começar a usar a API.

---

## 🛠️ Instalação

### 📋 Pré-requisitos

- **Windows 10/11** (64-bit)
- **.NET 8.0 Runtime** ou superior
- **SQL Server** (LocalDB incluído)
- **Ligação à Internet** (para validação de licenças)

### 📥 Download e Instalação

1. **Clone o Repositório**:
   ```bash
   git clone https://github.com/seu-usuario/CSMSageAPI.git
   cd CSMSageAPI
   ```

2. **Compile o Projeto**:
   ```bash
   dotnet build CSMSage/CSMSage.csproj
   ```

3. **Execute a Aplicação**:
   ```bash
   dotnet run --project CSMSage/CSMSage.csproj
   ```

### 🎯 Instalação Rápida

Para uma instalação mais simples, pode executar diretamente o executável:

1. Faça download do arquivo `CSMSage.exe`
2. Execute o arquivo
3. Siga as instruções de ativação da licença

---

## ⚙️ Configuração

### 🔑 Ativação da Licença

1. **Inicie a Aplicação**:
   - Execute o CSMSage
   - Será solicitada a chave de licença

2. **Introduza a Sua Chave**:
   - Cole a chave API obtida no portal beta
   - Clique em "Validar Licença"

3. **Confirmação**:
   - A aplicação validará a licença online
   - Após validação, estará pronto para usar

### 🌐 Configuração da API

1. **Inicie o Servidor API**:
   - Clique em "Iniciar API" na interface principal
   - O servidor iniciará na porta padrão (configurável)

2. **Aceda à Documentação**:
   - Abra o navegador em `http://localhost:porta/swagger`
   - Explore todos os endpoints disponíveis

3. **Teste a API**:
   - Use a interface Swagger para testar endpoints
   - Ou integre diretamente com a sua aplicação

### ⚙️ Configurações Avançadas

#### 🔧 Porta da API
```csharp
// Em ApiServer.cs
private const int DEFAULT_PORT = 8080; // Altere conforme necessário
```

#### 🗄️ Base de Dados
```csharp
// Em app.config
<connectionStrings>
    <add name="DefaultConnection" 
         connectionString="Data Source=(LocalDB)\MSSQLLocalDB;..." />
</connectionStrings>
```

---

## 📖 Documentação da API

### 🔗 Endpoints Principais

#### 👥 Gestão de Clientes
```
GET    /api/customers          # Listar clientes
POST   /api/customers          # Criar cliente
GET    /api/customers/{id}     # Obter cliente
PUT    /api/customers/{id}     # Atualizar cliente
DELETE /api/customers/{id}     # Eliminar cliente
```

#### 📦 Gestão de Produtos
```
GET    /api/items              # Listar produtos
POST   /api/items              # Criar produto
GET    /api/items/{id}         # Obter produto
PUT    /api/items/{id}         # Atualizar produto
DELETE /api/items/{id}         # Eliminar produto
```

#### 📊 Transações de Stock
```
GET    /api/stock-transactions  # Listar transações
POST   /api/stock-transactions  # Criar transação
GET    /api/stock-transactions/{id} # Obter transação
```

### 🔐 Autenticação

Todas as chamadas à API requerem autenticação via chave API:

```http
POST /api/customers
Content-Type: application/json
X-API-Key: SUA-CHAVE-API-AQUI

{
    "name": "Nome do Cliente",
    "email": "cliente@exemplo.com"
}
```

### 📝 Exemplo de Uso

#### JavaScript/Node.js
```javascript
const axios = require('axios');

const api = axios.create({
    baseURL: 'http://localhost:8080/api',
    headers: {
        'X-API-Key': 'SUA-CHAVE-API-AQUI',
        'Content-Type': 'application/json'
    }
});

// Criar cliente
const novoCliente = await api.post('/customers', {
    name: 'João Silva',
    email: 'joao@exemplo.com',
    phone: '+351 123 456 789'
});
```

#### Python
```python
import requests

headers = {
    'X-API-Key': 'SUA-CHAVE-API-AQUI',
    'Content-Type': 'application/json'
}

# Criar cliente
response = requests.post(
    'http://localhost:8080/api/customers',
    headers=headers,
    json={
        'name': 'João Silva',
        'email': 'joao@exemplo.com',
        'phone': '+351 123 456 789'
    }
)
```

#### C#
```csharp
using System.Net.Http;
using Newtonsoft.Json;

var client = new HttpClient();
client.DefaultRequestHeaders.Add("X-API-Key", "SUA-CHAVE-API-AQUI");

var novoCliente = new {
    name = "João Silva",
    email = "joao@exemplo.com",
    phone = "+351 123 456 789"
};

var json = JsonConvert.SerializeObject(novoCliente);
var content = new StringContent(json, Encoding.UTF8, "application/json");

var response = await client.PostAsync("http://localhost:8080/api/customers", content);
```

---

## 🔧 Desenvolvimento

### 🏗️ Estrutura do Projeto

```
CSMSageAPI/
├── CSMSage/                    # Aplicação principal
│   ├── Controllers/            # Controladores da API
│   ├── Models/                 # Modelos de dados
│   ├── Services/               # Serviços de negócio
│   ├── Helpers/                # Utilitários
│   └── Program.cs              # Ponto de entrada
├── Common/                     # Bibliotecas comuns
├── license_panel/              # Painel de gestão de licenças
└── README.md                   # Este arquivo
```

### 🛠️ Tecnologias Utilizadas

- **C# .NET 8.0**: Linguagem principal
- **ASP.NET Web API**: Framework da API
- **Entity Framework**: ORM para base de dados
- **Windows Forms**: Interface gráfica
- **Swagger/OpenAPI**: Documentação da API
- **Newtonsoft.Json**: Serialização JSON
- **SQL Server LocalDB**: Base de dados local

### 🔨 Compilação

```bash
# Restaurar dependências
dotnet restore

# Compilar em Debug
dotnet build --configuration Debug

# Compilar em Release
dotnet build --configuration Release

# Executar testes
dotnet test
```

### 📦 Dependências Principais

```xml
<PackageReference Include="Microsoft.AspNet.WebApi" Version="5.2.7" />
<PackageReference Include="Newtonsoft.Json" Version="13.0.3" />
<PackageReference Include="Swashbuckle" Version="5.6.0" />
```

---

## 📞 Suporte

### 🆘 Obter Ajuda

- **📧 Email**: suporte@csmsage.com
- **📞 Telefone**: +351 XXX XXX XXX
- **🌐 Website**: [www.csmsage.com](https://www.csmsage.com)
- **💬 GitHub Issues**: [Reportar Problemas](https://github.com/seu-usuario/CSMSageAPI/issues)

### 📚 Recursos Adicionais

- **📖 Documentação Completa**: [docs.csmsage.com](https://docs.csmsage.com)
- **🎥 Tutoriais em Vídeo**: [YouTube Channel](https://youtube.com/csmsage)
- **💬 Comunidade**: [Discord Server](https://discord.gg/csmsage)
- **📰 Blog**: [blog.csmsage.com](https://blog.csmsage.com)

### 🐛 Reportar Bugs

Ao reportar problemas, inclua:

1. **Versão do Sistema**: Windows 10/11
2. **Versão da Aplicação**: Visível no menu "Sobre"
3. **Passos para Reproduzir**: Descrição detalhada
4. **Logs de Erro**: Se disponíveis
5. **Screenshot**: Se aplicável

### 💡 Sugestões de Melhorias

Estamos sempre abertos a sugestões! Use as [GitHub Issues](https://github.com/seu-usuario/CSMSageAPI/issues) para:

- 🆕 Novas funcionalidades
- 🔧 Melhorias de performance
- 🎨 Melhorias de interface
- 📖 Melhorias na documentação

---

## 📄 Licença

Este projeto é propriedade da **CSMSage** e está protegido por direitos de autor. O uso é permitido apenas com licença válida.

### ⚖️ Termos de Uso

- ✅ Uso comercial permitido com licença
- ✅ Modificações permitidas para uso interno
- ❌ Redistribuição não autorizada
- ❌ Engenharia reversa proibida

### 🔒 Privacidade

- 🔐 Dados encriptados localmente
- 🌐 Validação de licenças online (sem dados pessoais)
- 📊 Estatísticas de uso anónimas
- 🚫 Nenhum dado pessoal enviado para servidores externos

---

<div align="center">

**Desenvolvido com ❤️ pela equipa CSMSage**

[![GitHub](https://img.shields.io/badge/GitHub-CSMSage-black?style=for-the-badge&logo=github)](https://github.com/seu-usuario/CSMSageAPI)
[![Website](https://img.shields.io/badge/Website-csmsage.com-blue?style=for-the-badge&logo=internet-explorer)](https://www.csmsage.com)
[![Email](https://img.shields.io/badge/Email-suporte@csmsage.com-red?style=for-the-badge&logo=gmail)](mailto:suporte@csmsage.com)

</div>
