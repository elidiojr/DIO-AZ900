# DIO-AZ900

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO.

## Conceitos Iniciais de Cloud com Azure

## Desafios de Projeto

### Desafio de Projeto 1: Computação em Nuvem

Este laboratório introduz o portal do Microsoft Azure, explicando a interface e funcionalidades básicas, como a personalização de idioma e aparência.

O foco principal está na seção “Computação”, onde são apresentados serviços relacionados à computação em nuvem, como máquinas virtuais, discos, redes virtuais (incluindo Bastiões/Jump Servers) e armazenamento. Também é destacado a importância de verificar o status dos serviços em “versão prévia”, que ainda não possuem SLA (Acordo de Nível de Serviço) e podem ser descontinuados sem aviso prévio.

Por fim, enfatiza a relevância da computação em nuvem no mercado de trabalho e incentiva os participantes a criarem uma conta gratuita no Azure para acompanhar os próximos laboratórios e se prepararem para a certificação AZ-900.

### Desafio de Projeto 2: Benefícios da Nuvem

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

### Desafio de Projeto 3: Tipos de Serviço de Nuvem

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
