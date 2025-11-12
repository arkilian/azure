# Primeiros Passos com Azure

## 🚀 Guia Prático para Iniciantes

Este guia irá ajudá-lo a dar os primeiros passos no Microsoft Azure de forma prática.

---

## 📋 Pré-requisitos

- Conta de email válida (pessoal ou corporativa)
- Cartão de crédito válido (para verificação de identidade - não será cobrado na conta gratuita)
- Navegador web moderno (Chrome, Edge, Firefox, Safari)

---

## 1️⃣ Criar Conta Gratuita do Azure

### Passo a Passo

1. **Acesse o site**
   - Vá para: https://azure.microsoft.com/pt-br/free/

2. **Inicie o cadastro**
   - Clique em "Iniciar gratuitamente" ou "Comece de graça"

3. **Entre com sua conta Microsoft**
   - Use uma conta existente ou crie uma nova
   - Pode ser conta pessoal (@outlook.com, @hotmail.com) ou corporativa

4. **Preencha seus dados**
   - Informações pessoais
   - Telefone para verificação
   - Cartão de crédito (apenas para verificação)

5. **Aceite os termos**
   - Leia e aceite o contrato
   - Clique em "Inscrever-se"

### O que está incluído?

✅ **$200 em créditos** para usar nos primeiros 30 dias  
✅ **12 meses de serviços gratuitos** incluindo:
   - 750 horas de VM B1S Windows ou Linux
   - 64 GB de armazenamento
   - 250 GB de SQL Database
   - E muito mais!

✅ **55+ serviços sempre gratuitos** incluindo:
   - Azure Functions (1 milhão de execuções/mês)
   - Azure Cosmos DB (1000 RU/s)
   - Azure DevOps (5 usuários)

📖 **Detalhes completos**: https://azure.microsoft.com/pt-br/free/free-account-faq/

---

## 2️⃣ Primeiro Acesso ao Portal do Azure

### Acessando o Portal

1. **Abra o portal**
   - Acesse: https://portal.azure.com
   - Faça login com suas credenciais

2. **Explore a interface**
   - **Menu lateral esquerdo**: Acesso aos serviços principais
   - **Barra superior**: Pesquisa, Cloud Shell, notificações
   - **Dashboard central**: Visão geral dos seus recursos

3. **Personalize seu dashboard**
   - Clique em "Dashboard"
   - Adicione tiles dos serviços que você mais usa
   - Arraste e organize conforme sua preferência

### Interface Principal

```
┌─────────────────────────────────────────────────────────┐
│ [≡] Portal do Azure    🔍    ☁️    🔔    👤           │
├─────────────────────────────────────────────────────────┤
│         │                                               │
│ [≡]     │        Dashboard / Visão Geral               │
│ Home    │                                               │
│ Todos   │  ┌──────────┐  ┌──────────┐  ┌──────────┐   │
│ recursos│  │ Recurso 1│  │ Recurso 2│  │ Recurso 3│   │
│         │  └──────────┘  └──────────┘  └──────────┘   │
│ Criar   │                                               │
│         │  [+ Criar um recurso]                        │
│         │                                               │
└─────────────────────────────────────────────────────────┘
```

---

## 3️⃣ Criar Seu Primeiro Recurso

### Exemplo: Criar um Grupo de Recursos

Os Grupos de Recursos são contêineres lógicos para organizar recursos relacionados.

#### Método 1: Pelo Portal

1. No menu lateral, clique em **"Grupos de recursos"**
2. Clique em **"+ Criar"** ou **"Adicionar"**
3. Preencha:
   - **Assinatura**: Selecione sua assinatura
   - **Nome do grupo**: `rg-meu-primeiro-projeto`
   - **Região**: `Brazil South` (São Paulo) ou `East US`
4. Clique em **"Revisar + criar"**
5. Clique em **"Criar"**

#### Método 2: Pelo Azure CLI

```bash
# Login no Azure
az login

# Criar grupo de recursos
az group create --name rg-meu-primeiro-projeto --location brazilsouth
```

#### Método 3: Pelo PowerShell

```powershell
# Login no Azure
Connect-AzAccount

# Criar grupo de recursos
New-AzResourceGroup -Name rg-meu-primeiro-projeto -Location brazilsouth
```

---

## 4️⃣ Explorar Serviços Principais

### A. Criar uma Conta de Armazenamento

1. No portal, clique em **"+ Criar um recurso"**
2. Procure por **"Conta de armazenamento"**
3. Clique em **"Criar"**
4. Preencha:
   - **Grupo de recursos**: `rg-meu-primeiro-projeto`
   - **Nome**: `stmeuprimeiroblob` (nome único globalmente)
   - **Região**: `Brazil South`
   - **Desempenho**: Standard
   - **Redundância**: LRS (Locally-redundant storage)
5. **Revisar + criar** → **Criar**

### B. Upload de um Arquivo

1. Vá até a conta de armazenamento criada
2. No menu lateral, clique em **"Contêineres"**
3. Clique em **"+ Contêiner"**
4. Nome: `meu-container`, Nível de acesso: Privado
5. Clique no contêiner criado
6. Clique em **"Carregar"**
7. Selecione um arquivo do seu computador
8. Clique em **"Carregar"**

---

## 5️⃣ Conhecer o Azure Cloud Shell

O Cloud Shell é um shell interativo no navegador para gerenciar recursos do Azure.

### Como Acessar

1. No portal do Azure, clique no ícone **Cloud Shell** (☁️) na barra superior
2. Escolha **Bash** ou **PowerShell**
3. Se for a primeira vez, crie uma conta de armazenamento para o Cloud Shell

### Comandos Úteis no Cloud Shell

```bash
# Listar todas as assinaturas
az account list --output table

# Listar grupos de recursos
az group list --output table

# Listar recursos em um grupo
az resource list --resource-group rg-meu-primeiro-projeto --output table

# Ver informações da conta de armazenamento
az storage account show --name stmeuprimeiroblob --resource-group rg-meu-primeiro-projeto
```

---

## 6️⃣ Instalar Ferramentas Locais

### Azure CLI (Linha de Comando)

#### Windows
```powershell
# Via winget
winget install -e --id Microsoft.AzureCLI

# Via MSI
# Baixe em: https://aka.ms/installazurecliwindows
```

#### macOS
```bash
brew update && brew install azure-cli
```

#### Linux (Ubuntu/Debian)
```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

**Verificar instalação:**
```bash
az --version
az login
```

### Azure PowerShell

```powershell
# Instalar módulo Az
Install-Module -Name Az -AllowClobber -Scope CurrentUser

# Importar módulo
Import-Module Az

# Conectar
Connect-AzAccount
```

### Visual Studio Code + Extensão Azure

1. Instale o Visual Studio Code: https://code.visualstudio.com/
2. Abra o VS Code
3. Vá em Extensões (Ctrl+Shift+X)
4. Procure por "Azure Tools"
5. Instale o pacote "Azure Tools for VS Code"

---

## 7️⃣ Boas Práticas Iniciais

### 🏷️ Use Tags

Tags ajudam a organizar e rastrear custos:

```bash
# Adicionar tags via CLI
az group update --name rg-meu-primeiro-projeto --tags Ambiente=Desenvolvimento Projeto=Aprendizado
```

### 💰 Configure Alertas de Custo

1. No portal, vá em **"Gerenciamento de Custos + Cobrança"**
2. Clique em **"Orçamentos"**
3. Clique em **"+ Adicionar"**
4. Configure:
   - Nome: `Alerta-Creditos-Gratuitos`
   - Valor: $200 (ou menor)
   - Alertas: 50%, 75%, 90%, 100%
   - Email para notificações

### 🔒 Ative Segurança

1. Vá em **"Microsoft Defender for Cloud"**
2. Siga as recomendações de segurança
3. Configure **autenticação multifator (MFA)**

### 🧹 Limpe Recursos Não Utilizados

Para evitar custos desnecessários, sempre delete recursos que não está usando:

```bash
# Deletar grupo de recursos e todos os recursos dentro dele
az group delete --name rg-meu-primeiro-projeto --yes --no-wait
```

---

## 8️⃣ Próximos Passos Práticos

### Projetos Simples para Praticar

1. **Criar um Site Estático**
   - Use Azure Storage Static Website
   - Upload de HTML/CSS/JS
   - Configure domínio customizado

2. **Deploy de uma Aplicação Web**
   - Use Azure App Service
   - Deploy via GitHub
   - Configure CI/CD

3. **Criar uma Máquina Virtual**
   - VM Linux ou Windows
   - Conecte via SSH ou RDP
   - Instale um servidor web

4. **Banco de Dados na Nuvem**
   - Azure SQL Database
   - Conecte com ferramenta de gerenciamento
   - Crie tabelas e execute queries

5. **Serverless com Azure Functions**
   - Crie uma função HTTP
   - Teste no navegador
   - Veja os logs

---

## 🆘 Ajuda e Suporte

### Quando Precisar de Ajuda

1. **Documentação oficial**: https://learn.microsoft.com/pt-br/azure/
2. **Microsoft Q&A**: https://learn.microsoft.com/pt-br/answers/
3. **Stack Overflow**: Tag [azure]
4. **Suporte do Azure**: No portal, clique em "?" → "Ajuda + suporte"

### Recursos Gratuitos de Aprendizagem

- **Microsoft Learn**: Módulos interativos gratuitos
- **Azure Quickstart Templates**: Templates prontos para usar
- **Azure Samples no GitHub**: Exemplos de código
- **Azure Friday**: Vídeos semanais

---

## ✅ Checklist de Primeiros Passos

- [ ] Criar conta gratuita do Azure
- [ ] Acessar o Portal do Azure
- [ ] Explorar a interface
- [ ] Criar um Grupo de Recursos
- [ ] Criar uma Conta de Armazenamento
- [ ] Upload de arquivo no Blob Storage
- [ ] Usar o Azure Cloud Shell
- [ ] Instalar Azure CLI localmente
- [ ] Configurar alerta de custos
- [ ] Adicionar tags aos recursos
- [ ] Explorar Microsoft Defender for Cloud
- [ ] Seguir um módulo do Microsoft Learn
- [ ] Criar seu primeiro projeto prático

---

**Parabéns por dar os primeiros passos no Azure! Continue praticando e explorando! 🎉**
