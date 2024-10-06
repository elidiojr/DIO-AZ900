# DIO-AZ900

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO.

## 🌐 **Módulo 1 - Conceitos Iniciais de Cloud com Azure**

### ⚡ *1.1 - Desafio de Projeto: Computação em Nuvem*

Este laboratório introduz o portal do Microsoft Azure, explicando a interface e funcionalidades básicas, como a personalização de idioma e aparência.

O foco principal está na seção “Computação”, onde são apresentados serviços relacionados à computação em nuvem, como máquinas virtuais, discos, redes virtuais (incluindo Bastiões/Jump Servers) e armazenamento. Também é destacado a importância de verificar o status dos serviços em “versão prévia”, que ainda não possuem SLA (Acordo de Nível de Serviço) e podem ser descontinuados sem aviso prévio.

Por fim, enfatiza a relevância da computação em nuvem no mercado de trabalho e incentiva os participantes a criarem uma conta gratuita no Azure para acompanhar os próximos laboratórios e se prepararem para a certificação AZ-900.

### ⚡ *1.2 - Desafio de Projeto: Benefícios da Nuvem*

Este laboratório explora os benefícios da nuvem, com foco especial nos Acordos de Nível de Serviço (SLAs). Entender o SLA é essencial para determinar o tempo de inatividade aceitável para os recursos e serviços na nuvem. Quanto mais "noves" no SLA, menor será o tempo de inatividade.

- **Exemplos de SLA:**
  - SLA de 99%: permite 1,68 horas de inatividade por semana.
  - SLA de 99,999%: permite apenas 5,26 minutos de inatividade por ano.

O laboratório também demonstra como o portal da nuvem oferece opções de disponibilidade e replicação que impactam diretamente no SLA e no custo.

- **Estratégias de Replicação:**
  - Zonas de disponibilidade
  - Conjuntos de dimensionamento
  - Tipos de replicação de dados: LRS, GRS, ZRS, GZRS

Essas escolhas influenciam diretamente a resiliência do sistema, o tempo de inatividade e o custo.

É importante lembrar que a alta disponibilidade e a resiliência na nuvem têm um custo. Portanto, é necessário analisar o propósito do recurso (produção, teste ou desenvolvimento) para definir o nível de SLA adequado, garantindo o melhor custo-benefício.

O profissional de nuvem precisa questionar as demandas e propor soluções otimizadas, explorando as diferentes possibilidades da plataforma e garantindo um SLA que atenda às necessidades do cliente.

### ⚡ *1.3 - Desafio de Projeto: Tipos de Serviço de Nuvem*

Este laboratório explora os diferentes tipos de serviços em nuvem, com foco em Infraestrutura como Serviço (IaaS), Plataforma como Serviço (PaaS) e Software como Serviço (SaaS). O objetivo é demonstrar como a escolha do tipo de serviço afeta o nível de controle e responsabilidade do usuário.

- **Pontos-chave:**
  - **Máquina virtual (IaaS):** O usuário tem controle total sobre a infraestrutura (sistema operacional, armazenamento, rede, etc.), o que torna a criação de uma máquina virtual um processo complexo, com diversas opções e configurações.
  - **Banco de dados SQL (PaaS):** O foco é no banco de dados, enquanto a Microsoft gerencia a infraestrutura subjacente. A criação de um banco de dados SQL no laboratório ilustra a simplicidade do processo.
  - **Calculadora de custos:** A ferramenta de cálculo de custos permite estimar o custo mensal com base nas configurações escolhidas, sendo essencial para planejar e gerenciar os gastos com serviços de nuvem.

- **Relação entre controle e responsabilidade:**
  - Quanto mais controle o usuário tem sobre a infraestrutura (IaaS), maior é sua responsabilidade pelo gerenciamento e manutenção.
  - O SaaS oferece o menor nível de controle, mas também a menor responsabilidade.

**Conclusões:**

- A escolha do tipo de serviço em nuvem depende das necessidades e do nível de controle desejado pelo usuário.
- É crucial entender as responsabilidades associadas a cada tipo de serviço.
- A calculadora de custos é uma ferramenta vital para gerenciar despesas com serviços em nuvem.

O laboratório reforça a importância de explorar as opções e configurações disponíveis antes de iniciar a criação de recursos na nuvem.

## 🌐 **Módulo 2 - Arquitetura e Serviços Azure**

### ⚡ *2.1 - Desafio de Projeto: Computação em Nuvem*

### ⚡ *2.2 - Desafio de Projeto: Computação e Rede*

Este laboratório explora os serviços de computação e rede do Microsoft Azure, com foco em Máquinas Virtuais, Áreas de Trabalho Virtual e Aplicações de Funções.

**Máquinas Virtuais**

O laboratório demonstra como criar uma máquina virtual (VM) no Azure, destacando as principais etapas de configuração:

- Nome, região, disponibilidade, tamanho, disco, rede e gerenciamento.
- Diferentes tipos de VMs e suas características, como:
  - Série D5
  - Série B
  - Série DC
  - Série H
- **Instância Spot:** Apresentada como uma forma de utilizar recursos não alocados do Azure a um custo reduzido. No entanto, a VM pode ser desligada caso outro cliente pague o preço cheio.
- Importância de habilitar a opção **“Excluir com VM”** para evitar discos órfãos que podem gerar custos desnecessários.
- Configuração de **Conjuntos de Dimensionamento (Scale Sets)** para escalonamento horizontal, com base em métricas como uso médio da CPU, limite mínimo, limite máximo e tempo de consulta.

**Área de Trabalho Virtual**

- Apresenta a **Área de Trabalho Virtual do Azure** como uma solução para oferecer um ambiente de trabalho remoto seguro e personalizado.
- Explicação sobre dois tipos de host:
  - **Host pessoal:** Dedicado a um único usuário.
  - **Pool de hosts:** Compartilhado entre múltiplos usuários.
- Aborda as opções de **balanceamento de carga** e **limite máximo de sessões** no contexto de pools de hosts.

**Aplicações de Funções**

O laboratório explora como criar um **aplicativo de função** no Azure, abordando:

- Configurações como nome, pilha de tempo de execução, hospedagem e plano de serviço.
- Diferentes linguagens de programação suportadas, como:
  - Node.js
  - Java
  - Python
  - .NET
- Introdução ao conceito **"sem servidor" (serverless)**, onde o aplicativo de função é executado sem a necessidade de gerenciar servidores.

**Dicas Importantes**

- Realizar atividades práticas no Azure, como criar VMs e aplicativos de função, para solidificar o entendimento dos conceitos e se preparar para a certificação AZ-900.
- Recomenda-se consultar a [documentação oficial do Azure](https://docs.microsoft.com/azure) e utilizar ferramentas de monitoramento e alertas para otimizar os serviços e garantir a segurança da infraestrutura.
- A prática contínua é essencial para se familiarizar com os recursos do Azure e seus diferentes cenários de uso.

### ⚡ *2.3 - Dominando o Armazenamento na Azure*

Este laboratório aborda conceitos e práticas de armazenamento na plataforma Azure, com foco em contas de armazenamento (Storage Accounts), migrações e ferramentas de gerenciamento.

**Contas de Armazenamento**

O laboratório demonstra a criação de uma conta de armazenamento no Azure, explorando suas funcionalidades principais, como:

- **Tipos de Armazenamento:**
  - Blobs
  - Arquivos
  - Filas
  - Tabelas
- **Importância de nome único para cada conta.**
- **Tipos de conta:** 
  - Standard
  - Premium
- **Redundância e opções de acesso.**

**Migrações para o Azure**

O laboratório apresenta o **serviço de migração do Azure**, que oferece ferramentas para:

- Avaliar, planejar e executar migrações de:
  - Servidores
  - Bancos de dados
  - Aplicativos web para a nuvem.
- **Funcionalidades:** 
  - Análise de dependências
  - Estratégias de migração
  - Análise financeira

**Ferramentas de Gerenciamento**

Duas ferramentas importantes foram destacadas no laboratório:

- **Azure Storage Explorer:**
  - Permite **visualizar, gerenciar e sincronizar arquivos** entre sua máquina local e a conta de armazenamento no Azure.
  - Interface gráfica fácil de usar.

- **AzCopy:**
  - Ferramenta de **linha de comando** para copiar e gerenciar dados entre sua máquina local e o Azure Storage.
  - Ideal para **transferências unilaterais**.
  - Funciona em diferentes sistemas operacionais: **Windows, Linux e Mac**.

**Detalhes Importantes**

- **Azure Databox:** O laboratório menciona que esta ferramenta **não está disponível** para assinaturas de treinamento.
- **Transferência de grandes volumes de dados:**
  - **Databox**
  - **Datadisk**
  - **Azure Import/Export**
  
- O **Azure Storage Explorer** oferece uma solução mais **visual e amigável** comparado ao AzCopy, sendo ideal para usuários que preferem uma interface gráfica.

**Conclusão**

O laboratório oferece uma visão geral prática e detalhada sobre as diferentes ferramentas e estratégias disponíveis para gerenciar e transferir dados dentro da plataforma Azure. Este conteúdo é valioso para quem busca se aprofundar na área de **cloud computing** e se preparar para o mercado de trabalho.

### ⚡ *2.4 - Desafio de Projeto: Entendendo sobre Segurança e Identidade na Azure*

Este laboratório aborda conceitos chave de identidade, acesso e segurança na plataforma Azure, com foco no **Microsoft Entra ID** (antigo Azure Active Directory) e no **Defender for Cloud**.

**Microsoft Entra ID**

1. Gerenciamento de Usuários
O **Microsoft Entra ID** centraliza o gerenciamento de usuários, permitindo a:

- **Criação e sincronização** com ambientes locais (on-premise)
- Controle de acesso, logs de atividades e redefinição de senhas

2. Domínios Personalizados
- Permite a personalização do **domínio de login** dos usuários com o nome da organização.

3. Licenciamento
- Recomenda-se utilizar os planos pagos **Premium P1** ou **P2** para acessar **recursos avançados** de gerenciamento e segurança.

4. RBAC (Controle de Acesso Baseado em Funções)
- Oferece ferramentas para **gerenciar permissões** relacionadas a ações dos usuários, mas não para o acesso a recursos diretamente.

5. Integração com Ambientes Locais
- O **Entra Connect** permite a sincronização de usuários e grupos entre o ambiente on-premise e o Azure, garantindo uma **gestão unificada**.

**Defender for Cloud**

1. Visão Unificada de Segurança
- O **Defender for Cloud** oferece um painel centralizado para **monitorar a postura de segurança** em diferentes plataformas, incluindo **Azure, AWS** e **GCP**.

2. Recomendações e Pontuação de Segurança
- Fornece **recomendações** para melhorar a segurança e acompanha a **pontuação de segurança** da sua infraestrutura.

3. DevOps Security
- Integra-se com ferramentas de **DevOps** como **GitHub** e **GitLab** para monitorar a segurança do código durante o processo de desenvolvimento.

4. Monitoramento de Recursos
- Oferece ferramentas para monitorar a segurança de recursos como:
  - **Máquinas virtuais**
  - **Serviços de aplicativos**
  - **Bancos de dados**
  - **Containers**

5. Gerenciamento de Ataques
- Funcionalidades para identificar e mitigar ataques, incluindo:
  - **Análise de vulnerabilidades**
  - **Detecção de intrusão**
  - **Resposta a incidentes**

**Benefícios do Defender for Cloud**

- **Simplificação do Gerenciamento de Segurança:** Visão unificada para monitorar a segurança em ambientes híbridos e multi-cloud.
- **Melhora da Postura de Segurança:** Recomendações e ferramentas para identificar e corrigir vulnerabilidades.
- **Gerenciamento Proativo de Riscos:** Detecção e resposta a incidentes de segurança de forma mais eficiente.

**Conclusão**

Este laboratório destaca a importância de soluções robustas de **identidade e segurança** no Azure, como o **Microsoft Entra ID** e o **Defender for Cloud**, para garantir a proteção de recursos e dados, e o gerenciamento eficiente do acesso a serviços e aplicações.

## 🌐 **Módulo 3 - Arquitetura e Serviços Azure**

### ⚡ *3.1 - Desafio de Projeto: Otimizando Custos no Azure*

A aula aborda a importância de **gerenciar custos** ao trabalhar com o Azure, especialmente durante a migração de ambientes on-premise para a nuvem. A principal ferramenta para isso é a **Calculadora de Custo Total de Propriedade (TCO)**, que permite **comparar os custos** do ambiente local com os custos estimados no Azure.

**1. Calculadora de Custo Total de Propriedade (TCO)**
- A calculadora TCO ajuda a **simular cenários de migração** e a comparar os custos do ambiente on-premise com o Azure.
- O usuário pode ajustar diferentes variáveis, como **modelos de licenças**, **reservas** e **tipos de instâncias** de máquinas virtuais.

**2. Calculadora de Preços do Azure**
- Esta calculadora permite obter **estimativas de custo** para diversos serviços, incluindo:
  - **Máquinas virtuais**
  - **Armazenamento**
  - **Bancos de dados**
  - **Serviços de rede**
- A aula ensina como **navegar pela ferramenta** e obter uma **visão geral dos custos mensais**.

**Gerenciamento de Custos e Faturamento (Cost Management + Billing)**
- A ferramenta **Cost Management + Billing** oferece um painel para **monitorar os gastos** no Azure.
- Funcionalidades principais:
  - **Identificação de alertas de custo**
  - **Recomendações do Advisor** para otimizar os custos

**Uso de Tags para Organizar Recursos**
- **Tags** (ou **Marcas**) permitem **categorizar** os recursos no Azure para facilitar a **organização e o gerenciamento** dos custos.
- A aula demonstra como:
  - Aplicar **tags** aos recursos
  - Usar **políticas** (policies) para definir **regras de aplicação de tags**

**Conclusão**
A aula fornece uma introdução completa ao **gerenciamento de custos** no Azure, destacando as ferramentas e recursos disponíveis para **controlar os gastos** e garantir uma **utilização eficiente e rentável** da nuvem.

### ⚡ *3.2 - Desafio de Projeto: Gerenciando Políticas em Acessos Azure*

A aula aborda conceitos chave de **governança** e **conformidade** dentro do Azure, focando em ferramentas e recursos importantes para garantir a **segurança** e o **cumprimento de regulamentações**.

**1. Portal de Confiança de Serviços**
- O portal [Service Trust Portal](https://servicetrust.microsoft.com) fornece informações sobre as **certificações**, **regulamentações** e **padrões de segurança** seguidos pela Microsoft.
- Essencial para empresas que precisam **demonstrar conformidade** durante auditorias.

**2. Bloqueios (Locks)**
- **Locks** impedem a **exclusão** ou **modificação** de recursos acidentalmente.
- Podem ser aplicados em nível de **Resource Group** ou diretamente no recurso.
  
**3. Microsoft Purview**
- Ferramenta abrangente para **gerenciar**, **proteger** e **monitorar dados** em ambientes como Microsoft 365 e Azure.
- Auxilia na conformidade com regulamentações como a **LGPD**.

**4. Políticas (Policies)**
- As **policies** são definidas em nível de **Management Group**, **assinatura** ou **Resource Group**.
- Estabelecem **regras** e **padrões** para gerenciar recursos, garantindo **consistência** e **segurança** dentro do ambiente Azure.

**5. Importância da Monitorização**
- É crucial **monitorar** o cumprimento das políticas e realizar **ajustes** para garantir que o ambiente está em **conformidade** com as regras definidas.

*Principais Aprendizados*

- A Microsoft oferece ferramentas e recursos para garantir a **segurança** e **conformidade** dentro do Azure.
- O **Portal de Confiança de Serviços** é fundamental para **demonstrar conformidade** com regulamentações e padrões de segurança.
- **Bloqueios** e **políticas** são mecanismos poderosos para **controlar o acesso** e **gerenciar recursos**.
- O **Microsoft Purview** auxilia na **gestão**, **proteção** e **monitoramento de dados**.
- A **monitorização constante** é essencial para garantir que as políticas estão sendo aplicadas corretamente e o ambiente está em **conformidade**.

### ⚡ *3.3 - Desafio de Projeto: Ferramentas de Implantação na Nuvem*

A aula explora a **criação** e **gerenciamento de recursos** no Azure, com ênfase no uso do **Cloud Shell**, **PowerShell** e na importância da **automação** com **Bicep** e **Azure Arc**.

**Portal Intuitivo**
- O portal Azure é projetado para facilitar a criação de recursos sem a necessidade de comandos, tornando-o **acessível a iniciantes**. Isso promove uma experiência de usuário mais amigável e direta.

**Cloud Shell**
- A ferramenta **Cloud Shell** é crucial para usuários que desejam executar comandos rapidamente. Ela se **integra diretamente ao portal** e facilita o gerenciamento de recursos, eliminando a necessidade de abrir um terminal separado.

**Automação com Bicep**
- O uso do **Bicep** reduz significativamente a complexidade e a quantidade de linhas de código necessárias para criar recursos, facilitando a automação. Especialmente para iniciantes, o Bicep é uma alternativa mais amigável em comparação ao ARM Template, que pode ser mais intimidador.

**Gerenciamento Multicloud com Azure Arc**
- O **Azure Arc** é uma solução poderosa para **gerenciar recursos** que não estão apenas no Azure, mas também em outras nuvens (multicloud), centralizando a administração e melhorando a **eficiência operacional**.

**Eficiência na Criação de Recursos**
- A criação de recursos em **lote** pode ser uma estratégia mais eficiente, evitando a criação manual repetitiva e acelerando o processo de provisionamento.

**Flexibilidade nos Comandos**
- A possibilidade de usar tanto **PowerShell** quanto **CLI** no Cloud Shell oferece flexibilidade aos desenvolvedores, permitindo que trabalhem com a interface com a qual se sentem mais confortáveis.

**Exploração e Aprendizado**
- A prática em **ambientes de laboratório** e a exploração de recursos como o **Azure Arc** e **Bicep** são essenciais para entender as capacidades do Azure e melhorar as **habilidades técnicas**.

**Conclusão**

Essa aula oferece uma visão abrangente das diferentes maneiras de **criar** e **gerenciar recursos no Azure**, destacando a importância da **automação** e do **gerenciamento multicloud**. Ele serve como um guia essencial tanto para iniciantes quanto para profissionais que buscam maximizar a eficiência no uso da plataforma.

### ⚡*3.4 - Monitoramento Inteligente com o Azure*

O laboratório aborda a **importância do monitoramento** na infraestrutura do Azure, destacando ferramentas como o **Azure Monitor**, **Azure Service Health** e **Azure Advisor**.

**Azure Monitor**

O **Azure Monitor** fornece uma visão abrangente do ambiente, permitindo monitorar a **saúde** e o **desempenho** de recursos como máquinas virtuais, aplicações, armazenamento e rede. Ele oferece vários recursos, como:

- **Monitoramento de saúde e performance**: Acompanha o estado e a performance dos recursos.
- **Insights**: Fornece análise de dados para identificar **padrões** e **tendências**.
- **Criação de alertas**: Permite a criação de **notificações personalizadas** para eventos específicos.

**Azure Service Health**

O **Azure Service Health** é uma ferramenta essencial para verificar a **saúde dos serviços do Azure**, identificando:

- **Problemas** em serviços.
- **Manutenções planejadas**.
- **Recomendações de saúde e segurança**.

É crucial para verificar a **disponibilidade de serviços** antes de reportar problemas, evitando falsas reclamações e melhorando o suporte técnico.

**Azure Advisor**

O **Azure Advisor** oferece recomendações personalizadas para otimizar o uso de recursos. Suas funcionalidades incluem:

- **Melhoria de segurança**, confiabilidade, desempenho e custo.
- **Análise do ambiente** para identificar áreas de aprimoramento.
- **Sugestão de ações** para melhorar a performance e a eficiência da infraestrutura.

**Conclusão**

O monitoramento é fundamental para garantir um ambiente **saudável**, **seguro** e **eficiente**. Através das ferramentas de monitoramento do Azure, como o Azure Monitor, Azure Service Health e Azure Advisor, é possível **identificar problemas** rapidamente, **otimizar recursos** e melhorar a experiência dos usuários finais.




