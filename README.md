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
- [🚀 Obter Chave API Beta](#-obter-chave-api-beta)
- [⚙️ Configuração](#️-configuração)
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

---

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

---

## 📞 Suporte

### 🆘 Obter Ajuda

- **📧 Email**: opmeso@gmail.com
- **📞 Telefone**: +351 XXX XXX XXX
- **💬 GitHub Issues**: [Reportar Problemas](https://github.com/mesofranico/50cAPI/issues)

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
