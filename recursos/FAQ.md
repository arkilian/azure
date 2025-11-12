# Perguntas Frequentes (FAQ) - Azure Fundamentals

## 💰 Custos e Conta

### Preciso pagar para aprender Azure?
Não! A Microsoft oferece:
- **$200 em créditos gratuitos** para os primeiros 30 dias
- **12 meses de serviços gratuitos** populares
- **55+ serviços sempre gratuitos**

Você só precisa de um cartão de crédito para verificação de identidade, mas não será cobrado enquanto usar apenas os recursos gratuitos.

### O que acontece depois que meus créditos acabarem?
Após os 30 dias ou quando seus $200 de crédito acabarem (o que vier primeiro), você precisará atualizar para uma assinatura paga para continuar usando serviços pagos. No entanto:
- Serviços gratuitos continuam gratuitos
- Você não será cobrado automaticamente - precisa aprovar a atualização
- Pode continuar aprendendo com os recursos sempre gratuitos

### Como evito cobranças inesperadas?
1. Configure alertas de custo no portal
2. Use apenas recursos da camada gratuita
3. Sempre delete recursos que não está usando
4. Monitore seus gastos regularmente no Cost Management
5. Não atualize para assinatura paga sem querer

### Posso usar Azure para fins comerciais com a conta gratuita?
A conta gratuita é principalmente para desenvolvimento e teste. Para produção, você deve usar uma assinatura paga apropriada.

---

## 🎓 Aprendizagem e Certificação

### Quanto tempo leva para aprender Azure Fundamentals?
Depende do seu ritmo e conhecimento prévio:
- **Iniciantes em cloud:** 6-10 semanas (2-3 horas/semana)
- **Com experiência em TI:** 3-6 semanas (2-3 horas/semana)
- **Preparação intensiva para AZ-900:** 2-4 semanas (5-10 horas/semana)

### Preciso saber programação para aprender Azure?
Não para os fundamentos! Azure Fundamentals é focado em conceitos, não em programação. No entanto, conhecimento básico de:
- Redes (IP, DNS, firewall)
- Sistemas operacionais (Windows/Linux)
- Bancos de dados
pode ser útil.

### A certificação AZ-900 vale a pena?
Sim, especialmente se você:
- Está começando carreira em cloud
- Quer validar conhecimentos básicos
- Precisa de credencial reconhecida
- Trabalha ou quer trabalhar com Azure

**Nota:** AZ-900 é certificação de nível fundamental. Para funções técnicas, considere certificações de Associate ou Expert.

### Qual a diferença entre este guia e a documentação oficial?
Este guia:
- Está organizado para aprendizagem sequencial
- Inclui materiais complementares
- Tem foco em iniciantes de língua portuguesa
- Fornece exemplos práticos simplificados

A documentação oficial:
- É mais técnica e completa
- Serve como referência detalhada
- É atualizada constantemente

Use os dois juntos para melhor aprendizado!

---

## 🛠️ Questões Técnicas

### Qual região do Azure devo usar?
Para Brasil: **Brazil South (São Paulo)**
- Menor latência
- Conformidade com dados brasileiros
- Alguns serviços podem custar mais

Alternativas populares:
- **East US** - Muitos serviços, geralmente mais barato
- **West Europe** - Boa opção para Europa/África

**Dica:** Para aprendizado, use qualquer região. Para produção, escolha baseado em latência, custos e conformidade.

### O que fazer quando um recurso não está disponível na minha região?
1. Use outra região próxima
2. Verifique o [Azure Products by Region](https://azure.microsoft.com/pt-br/explore/global-infrastructure/products-by-region/)
3. Para aprendizado, isso raramente é problema

### Azure CLI ou PowerShell - qual usar?
**Azure CLI:**
- Sintaxe mais simples
- Multiplataforma (Windows, Mac, Linux)
- Mais popular na comunidade
- Recomendado para iniciantes

**Azure PowerShell:**
- Integrado com ecossistema PowerShell
- Melhor para quem já conhece PowerShell
- Mais usado em ambientes Windows Server

**Recomendação:** Comece com Azure CLI, aprenda PowerShell se necessário.

### Posso usar Azure no meu computador?
Azure é serviço de nuvem - recursos rodam em datacenters da Microsoft, não no seu computador. Você:
- **Acessa** via browser (Portal do Azure)
- **Gerencia** via CLI/PowerShell local
- **Desenvolve** aplicações localmente e faz deploy no Azure

---

## 📚 Recursos e Ferramentas

### Preciso instalar algo?
Para começar: **Não!** Use apenas o Portal do Azure no navegador.

Opcionalmente, instale:
- **Azure CLI** - Linha de comando
- **Visual Studio Code + extensões Azure** - IDE
- **Azure PowerShell** - Scripts PowerShell
- **Azure Storage Explorer** - Gerenciar storage

### A documentação está em português?
Sim e não:
- **Documentação principal**: Boa parte está em português
- **Artigos novos**: Primeiro em inglês, depois traduzidos
- **Tutoriais**: Mistura de português e inglês
- **Microsoft Learn**: Muitos módulos em português

**Dica:** Use tradução automática do navegador quando necessário.

### Onde encontro código de exemplo?
- [Azure Samples no GitHub](https://github.com/Azure-Samples)
- [Microsoft Learn - módulos práticos](https://learn.microsoft.com/pt-br/training/)
- [Azure Quickstart Templates](https://azure.microsoft.com/resources/templates/)
- Documentação oficial de cada serviço

---

## 🚀 Prática e Projetos

### O que posso construir com a conta gratuita?
Exemplos:
- Site estático (Static Web App)
- API REST (Azure Functions)
- Aplicação web (App Service)
- Bot simples (Bot Service)
- Banco de dados pequeno (SQL Database)
- Sistema de arquivos (Storage)

### Como sei se vou gastar meus créditos?
1. Use a **Calculadora de Preços** antes de criar recursos
2. Prefira recursos na camada **Free** ou **Basic**
3. Configure **alertas de custo**
4. Monitore gastos diariamente no início

### Posso compartilhar minha conta Azure com colegas de estudo?
**Não recomendado!** Cada pessoa deve ter sua própria conta porque:
- Questões de segurança
- Controle de créditos
- Prática individual é importante
- Violação dos termos de uso

Para estudar em grupo, cada um cria sua conta e compartilha apenas conhecimento e códigos.

### Meu recurso falhou ao criar. O que fazer?
Causas comuns:
1. **Nome já existe** - Use nome único globalmente
2. **Quota excedida** - Verifique limites da conta
3. **Região não suporta** - Tente outra região
4. **Erro de permissão** - Verifique se tem acesso necessário

Sempre leia a mensagem de erro - ela geralmente explica o problema.

---

## 🎯 Carreira e Próximos Passos

### Após Azure Fundamentals, qual certificação fazer?
Depende do seu interesse:

**Desenvolvimento:**
- AZ-204: Azure Developer Associate

**Administração:**
- AZ-104: Azure Administrator Associate

**Arquitetura:**
- AZ-305: Azure Solutions Architect Expert (requer AZ-104)

**Dados:**
- DP-900: Data Fundamentals
- DP-203: Data Engineer Associate

**IA:**
- AI-900: AI Fundamentals
- AI-102: AI Engineer Associate

### Quais são as carreiras em Azure?
- **Azure Developer** - Desenvolve aplicações na nuvem
- **Azure Administrator** - Gerencia infraestrutura Azure
- **Azure Solutions Architect** - Projeta soluções complexas
- **Azure DevOps Engineer** - Automação e CI/CD
- **Azure Data Engineer** - Pipelines de dados
- **Azure Security Engineer** - Segurança e conformidade

### Preciso de todas as certificações?
Não! Foque na área que mais te interessa. A maioria dos profissionais tem 1-3 certificações relevantes para sua função.

---

## ⚠️ Problemas Comuns

### "Não consigo criar conta gratuita"
Possíveis soluções:
- Verifique se já usou esse email antes
- Use cartão de crédito internacional válido
- Tente navegador diferente/modo anônimo
- Verifique se seu país está suportado

### "Erro 403 - Forbidden" no portal
Causas:
- Sem permissões necessárias
- Assinatura suspensa/expirada
- Política da organização bloqueando

Solução: Verifique suas permissões com administrador da conta.

### "Quota exceeded" ao criar recurso
Conta gratuita tem limites. Soluções:
- Delete recursos antigos
- Solicite aumento de quota (alguns casos)
- Use recursos alternativos
- Aguarde renovação mensal de quotas

### Portal Azure está lento
Possíveis causas:
- Muitos recursos abertos
- Conexão lenta
- Problemas temporários do Azure

Soluções:
- Limpe cache do navegador
- Use modo anônimo
- Verifique [Azure Status](https://status.azure.com)
- Tente outro navegador

---

## 🌐 Comunidade e Suporte

### Onde posso fazer perguntas?
- [Microsoft Q&A](https://learn.microsoft.com/answers/)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/azure)
- [Reddit - r/AZURE](https://reddit.com/r/AZURE)
- Grupos de usuários locais
- Tech Community da Microsoft

### Como contribuo com a comunidade?
- Responda perguntas em fóruns
- Escreva artigos/tutoriais
- Compartilhe projetos no GitHub
- Apresente em meetups
- Ajude colegas de estudo

### Existe suporte oficial gratuito?
A conta gratuita inclui:
- Documentação completa
- Fóruns da comunidade
- Suporte de faturamento

Suporte técnico pago está disponível em diferentes níveis.

---

## 📖 Dicas de Estudo

### Como memorizar tantos serviços?
**Não tente decorar!** Foque em:
1. **Entender conceitos** fundamentais
2. **Saber categorias** (computação, rede, storage, etc.)
3. **Conhecer casos de uso** de cada serviço
4. **Praticar** com serviços principais

Com o tempo e prática, você lembrará naturalmente.

### Melhor horário para estudar?
O horário que você consegue ser **consistente**:
- Manhã: Mente fresca, menos distrações
- Noite: Após trabalho, mais calmo
- Fins de semana: Sessões mais longas

**Importante:** Regularidade > Quantidade de horas

### Como não desistir?
1. Estabeleça metas realistas
2. Estude com outras pessoas
3. Celebre pequenas vitórias
4. Varie os métodos de estudo
5. Aplique o que aprende em projetos
6. Lembre-se do seu objetivo

---

**Não encontrou sua pergunta? Crie uma issue no repositório ou procure ajuda na comunidade!** 🤝
