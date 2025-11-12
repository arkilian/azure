# Glossário Azure - Termos Importantes

## 🔤 Termos Fundamentais

### Computação em Nuvem (Cloud Computing)

**Cloud Computing**
- Entrega de serviços de computação pela Internet, incluindo servidores, armazenamento, bancos de dados, redes, software e análises.

**IaaS (Infrastructure as a Service)**
- Infraestrutura como Serviço: Fornece infraestrutura de TI virtualizada pela Internet.
- Exemplo: Azure Virtual Machines

**PaaS (Platform as a Service)**
- Plataforma como Serviço: Fornece plataforma de desenvolvimento e implantação pela Internet.
- Exemplo: Azure App Service

**SaaS (Software as a Service)**
- Software como Serviço: Fornece aplicativos pela Internet sob demanda.
- Exemplo: Microsoft 365

### Modelos de Nuvem

**Nuvem Pública**
- Recursos de nuvem pertencentes e operados por provedores de serviços de nuvem de terceiros.

**Nuvem Privada**
- Recursos de nuvem usados exclusivamente por uma organização.

**Nuvem Híbrida**
- Combinação de nuvens públicas e privadas.

## 🏗️ Conceitos do Azure

### Estrutura Organizacional

**Azure Account (Conta Azure)**
- Identidade que fornece acesso aos serviços do Azure.

**Subscription (Assinatura)**
- Contêiner lógico usado para provisionar recursos no Azure.
- Unidade de faturamento.

**Resource Group (Grupo de Recursos)**
- Contêiner que mantém recursos relacionados para uma solução Azure.

**Resource (Recurso)**
- Item gerenciável disponível no Azure (VM, banco de dados, rede virtual, etc.).

**Region (Região)**
- Área geográfica que contém um ou mais datacenters.

**Availability Zone (Zona de Disponibilidade)**
- Datacenters fisicamente separados dentro de uma região do Azure.

**Azure Resource Manager (ARM)**
- Serviço de implantação e gerenciamento para o Azure.

### Identidade e Acesso

**Azure Active Directory (Azure AD / Entra ID)**
- Serviço de gerenciamento de identidade e acesso baseado em nuvem da Microsoft.

**Tenant (Locatário)**
- Instância dedicada do Azure AD que uma organização recebe ao criar relacionamento com a Microsoft.

**Identity (Identidade)**
- Objeto que pode ser autenticado (usuário, aplicativo, serviço).

**Authentication (Autenticação)**
- Processo de verificar a identidade de um usuário ou serviço.

**Authorization (Autorização)**
- Processo de determinar o nível de acesso que uma identidade autenticada tem.

**RBAC (Role-Based Access Control)**
- Controle de Acesso Baseado em Função: Sistema de autorização que fornece gerenciamento de acesso refinado.

**Service Principal**
- Identidade criada para uso com aplicativos, serviços hospedados e ferramentas automatizadas.

**Managed Identity**
- Identidade gerenciada automaticamente pelo Azure para autenticar em serviços Azure.

## 💾 Serviços de Computação

**Virtual Machine (VM / Máquina Virtual)**
- Emulação de um computador físico.

**VM Scale Set**
- Conjunto de VMs idênticas com balanceamento de carga automático.

**App Service**
- Serviço de hospedagem gerenciado para aplicativos web e APIs.

**Azure Functions**
- Serviço de computação serverless orientado a eventos.

**Azure Container Instances (ACI)**
- Serviço para executar containers sem gerenciar servidores.

**Azure Kubernetes Service (AKS)**
- Serviço de orquestração de containers gerenciado usando Kubernetes.

**Azure Batch**
- Serviço para executar aplicações paralelas e de HPC em larga escala.

## 🌐 Serviços de Rede

**Virtual Network (VNet)**
- Rede isolada no Azure para seus recursos.

**Subnet (Sub-rede)**
- Segmento de uma rede virtual.

**Network Security Group (NSG)**
- Grupo de regras de segurança que filtram o tráfego de rede.

**Load Balancer**
- Distribui tráfego de entrada entre várias VMs.

**Application Gateway**
- Balanceador de carga de camada 7 (HTTP/HTTPS).

**VPN Gateway**
- Gateway que envia tráfego criptografado entre rede virtual Azure e local.

**ExpressRoute**
- Conexão privada dedicada entre infraestrutura local e Azure.

**Azure DNS**
- Serviço de hospedagem DNS.

**Content Delivery Network (CDN)**
- Rede de servidores distribuída que entrega conteúdo com baixa latência.

## 💽 Serviços de Armazenamento

**Storage Account**
- Conta que fornece namespace exclusivo para dados do Azure Storage.

**Blob Storage**
- Armazenamento de objetos otimizado para grandes quantidades de dados não estruturados.

**File Storage**
- Compartilhamentos de arquivos gerenciados na nuvem (protocolo SMB).

**Queue Storage**
- Serviço de armazenamento de mensagens para comunicação entre componentes.

**Table Storage**
- Armazenamento NoSQL de dados estruturados.

**Disk Storage**
- Discos gerenciados para VMs.

**Archive Storage**
- Camada de armazenamento de baixo custo para dados raramente acessados.

**Data Lake Storage**
- Repositório de dados massivo para análise de big data.

## 🗄️ Serviços de Banco de Dados

**Azure SQL Database**
- Banco de dados relacional gerenciado baseado em SQL Server.

**Azure Cosmos DB**
- Banco de dados NoSQL multimodelo distribuído globalmente.

**Azure Database for MySQL**
- Banco de dados MySQL gerenciado.

**Azure Database for PostgreSQL**
- Banco de dados PostgreSQL gerenciado.

**Azure Cache for Redis**
- Cache gerenciado baseado em Redis.

**Azure Synapse Analytics**
- Serviço de análise que une data warehouse e big data.

## 🔐 Segurança

**Azure Security Center / Microsoft Defender for Cloud**
- Gerenciamento unificado de segurança e proteção contra ameaças.

**Azure Key Vault**
- Serviço para armazenar e acessar segredos com segurança.

**Azure DDoS Protection**
- Proteção contra ataques de negação de serviço distribuído.

**Azure Firewall**
- Firewall de rede gerenciado baseado em nuvem.

**Azure Sentinel**
- Solução SIEM (Security Information and Event Management) nativa da nuvem.

## 📊 Monitoramento e Gerenciamento

**Azure Monitor**
- Serviço abrangente para coletar, analisar e agir com telemetria.

**Log Analytics**
- Ferramenta para editar e executar consultas de log.

**Application Insights**
- Serviço de APM (Application Performance Management).

**Azure Advisor**
- Serviço de recomendações personalizadas de melhores práticas.

**Azure Service Health**
- Informações personalizadas sobre saúde dos serviços Azure.

**Azure Policy**
- Serviço para criar, atribuir e gerenciar políticas.

**Azure Blueprints**
- Definições reutilizáveis de ambientes Azure.

**Management Groups**
- Contêineres para gerenciar acesso, políticas e conformidade em várias assinaturas.

## 💰 Custos e Faturamento

**Cost Management**
- Ferramentas para monitorar, alocar e otimizar custos do Azure.

**Pricing Calculator**
- Ferramenta para estimar custos de serviços Azure.

**TCO Calculator**
- Calculadora de Custo Total de Propriedade.

**Budget**
- Limites de gastos configurados para receber alertas.

**Tags**
- Pares nome-valor para organizar recursos e visualizar custos consolidados.

## 🚀 DevOps e Desenvolvimento

**Azure DevOps**
- Conjunto de serviços de desenvolvimento colaborativo.

**Azure Repos**
- Repositórios Git ou TFVC.

**Azure Pipelines**
- Serviço de CI/CD.

**Azure Boards**
- Ferramenta de rastreamento de trabalho ágil.

**Azure Artifacts**
- Repositório de pacotes (Maven, npm, NuGet, etc.).

**Azure Test Plans**
- Ferramentas de teste manual e exploratório.

**ARM Template**
- Arquivo JSON que define infraestrutura e configuração do projeto.

**Bicep**
- Linguagem declarativa para implantar recursos do Azure.

## 🌍 Outros Conceitos Importantes

**SLA (Service Level Agreement)**
- Acordo de Nível de Serviço: Compromisso de disponibilidade e desempenho.

**RPO (Recovery Point Objective)**
- Objetivo de Ponto de Recuperação: Perda máxima de dados aceitável.

**RTO (Recovery Time Objective)**
- Objetivo de Tempo de Recuperação: Tempo máximo de inatividade aceitável.

**Geo-Redundancy**
- Replicação de dados em várias regiões geográficas.

**Elasticity**
- Capacidade de escalar recursos automaticamente com base na demanda.

**Scalability**
- Capacidade de adicionar recursos para lidar com aumento de carga.

**High Availability**
- Sistema que opera continuamente sem falhas por longo tempo.

**Disaster Recovery**
- Conjunto de políticas para recuperar sistemas após desastre.

**Compliance**
- Conformidade com regulamentos e padrões (GDPR, HIPAA, etc.).

## 🎓 Termos de Certificação

**AZ-900**
- Certificação Azure Fundamentals.

**Learning Path**
- Coleção de módulos de treinamento relacionados.

**Sandbox**
- Ambiente de prática temporário fornecido pelo Microsoft Learn.

**Hands-on Lab**
- Exercício prático com recursos reais do Azure.

---

**Dica**: Use este glossário como referência rápida enquanto estuda! 📖
