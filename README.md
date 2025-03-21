### PRINCÍPIOS E DESIGN E PRÁTICAS RECOMENDADAS AWS WELL-ARCHITECTED

**Objetivo:** Este documento tem o objetivo de ajudar estudantes a melhorar a compreensão dos conceitos para realização do exame SAA-C03.

## O que é o Well-Architected?

O AWS Well-Architected Framework é um conjunto de práticas recomendadas e diretrizes de arquitetura desenvolvido pela Amazon Web Services (AWS) para ajudar os clientes a construir e operar sistemas seguros, confiáveis, eficientes e econômicos na nuvem AWS.

Em poucas palavras, é um guia geral para construir boas arquiteturas de nuvem da Amazon Web Services.

## Para que serve?

Serve para tomar decisões informadas sobre arquiteturas dos clientes, compreender o impacto das decisões de design e ficar ciente dos riscos existentes e das formas de mitigá-los, e assim controlar o impacto sobre os negócios.

Em quatro palavras, ajuda os arquitetos de nuvem a avaliar e aprimorar suas arquiteturas e entender melhor como as decisões de design podem afetar os negócios.

* Avaliar
* Aprimorar
* Design
* Arquiteturas

## Princípios Gerais de Design

* Parar de adivinhar as necessidades das capacidades
* Testar os sistemas em escala de produção
* Automatizar para facilitar experimentos de arquitetura
* Permitir que as arquiteturas evoluam
* Impulsionar arquitetura usando dados
* Aprimorar por meio de dias de testes

## Linha do tempo

O Framework AWS Well-Architected evoluiu desde 2012, com adições de pilares, lentes, suporte regional e ferramentas de autoatendimento, para ajudar os clientes a construir e operar cargas de trabalho seguras, confiáveis, eficientes e sustentáveis na AWS.

* 2012: Início do AWS Well-Architected.
* 2013: Análises de arquitetos de soluções da AWS.
* 2014: Perguntas sobre os pilares.
* 2015: Publicação do Framework.
* 2016: Pilar de excelência operacional.
* 2017: Lentes para AWS Partners.
* 2018: Autoatendimento e planos de melhoria.
* 2019: Lançamentos regionais.
* 2020: Atualização do Framework e proprietário da análise.
* 2021: Sustentabilidade e mais lentes.
* 2022: AWS GovCloud e AWS Trusted Advisor.
* ??? Última atualização github pages

## PILARES DO WELL ARCHITECTED

Mnemônico: 2E2SCO

Excelência, Eficiência, Segurança, Sustentabilidade, Confiabilidade e Otimização

Pense nos pilares como um guia para construir sistemas na AWS que sejam:

* Bem gerenciados (Pilar de excelência operacional)
* Seguros (Pilar de segurança)
* Confiáveis (Pilar de confiabilidade)
* Rápidos (Pilar de eficiência de desempenho)
* Econômicos (Pilar otimização de custos)
* Responsabilidade social (Pilar de sustentabilidade)

## EXCELÊNCIA OPERACIONAL

### O que é?

Excelência operacional é a capacidade de oferecer suporte ao desenvolvimento e executar cargas de trabalho de forma eficaz, obter informações sobre as operações e melhorar continuamente os processos e procedimentos de suporte para fornecer valor comercial.

* **Foco Principal:** Automatizar e otimizar processos para garantir a eficiência e a confiabilidade das operações ao longo do ciclo de vida da aplicação.
* **Âmbito:** Ciclo de vida completo da aplicação.
* **Objetivo:** Reduzir erros humanos, automatizar processos, garantir a confiabilidade.
* **Métricas:** Tempo de implantação, taxa de falhas em implantações, tempo de recuperação (RTO/RPO), tempo médio de resolução (MTTR).
* **Uso prático:** Utilizar o AWS CloudFormation para provisionar automaticamente um ambiente de desenvolvimento, teste e produção, garantindo consistência e reduzindo erros de configuração.
* **Diferenças Notáveis:** Abrange o ciclo de vida completo da aplicação. Foca em métricas de processo.

### Princípio de design Excelência Operacional

* Executar operações como código
* Fazer alterações frequentes, pequenas e reversíveis
* Refinar os procedimentos de operações com frequência
* Prever falhas, testar cenários e valide a compreensão
* Aprender com todas as falhas operacionais

### Práticas recomendadas de Excelência Operacional

* Organização
* Preparar
* Operar
* Evoluir

### Conceitos Chave:

* Infraestrutura como código (IaC) para provisionamento consistente e repetível.
* Automação de implantações (CI/CD) para entrega rápida e confiável.
* Monitoramento proativo da saúde do sistema para detecção precoce de problemas.
* Gerenciamento eficaz de incidentes para minimizar o tempo de inatividade.
* Planejamento e execução de recuperação de desastres para garantir a continuidade dos negócios.

### Resumo:

Trata-se de como você opera, mantém e evolui sua infraestrutura e aplicações, com ênfase na automação e na melhoria contínua.

### Definição em uma frase:

Estabelecer e aprimorar processos para garantir a execução eficiente e confiável de sistemas e operações.

### Definição em uma palavra:

Automação.

### Palavras Chave:

Automação, monitoramento, melhoria contínua, entrega de valor, reação a eventos e alterações, definição de padrões, executar operações como código, antecipar e prever falhas, anotar e documentar, fazer alterações pequenas e reversíveis, aprender com as falhas, gerenciamento de mudanças, IaC, CI/CD.

## EFICIÊNCIA DE DESEMPENHO

### O que é?

A eficiência de desempenho concentra-se no uso eficiente de recursos de computação para atender aos requisitos e em como manter a eficiência à medida que a demanda muda e as tecnologias evoluem.

* **Foco Principal:** Otimizar o uso de recursos da AWS para entregar o melhor desempenho possível, de forma escalável e adaptável à demanda.
* **Âmbito:** Desempenho da aplicação em tempo de execução.
* **Objetivo:** Maximizar a velocidade e a capacidade de resposta da aplicação.
* **Métricas:** Latência, throughput, utilização de CPU/memória, taxa de erros.
* **Uso prático:** Implementar o Amazon CloudFront para distribuir conteúdo estático e dinâmico, reduzindo a latência para usuários em diferentes regiões.
* **Diferenças Notáveis:** Concentra-se na otimização do desempenho em tempo de execução. Foca em métricas de sistema.

### Princípio de design Eficiência de Desempenho

* Democratiza tecnologias avançadas
* Ter alcance global em minutos
* Usar arquiteturas sem servidor
* Fazer experimentos com mais frequência
* Considerar afinidade mecânica

### Práticas recomendadas de Eficiência de Desempenho

* Seleção
* Análise
* Monitoramento
* Concessões

### Conceitos Chave:

* Seleção de tipos de instâncias: EC2, Lambda.
* Escalabilidade: Auto Scaling, Elastic Load Balancing.
* Caching: Amazon CloudFront, ElastiCache.
* Otimização de rede: VPC, Direct Connect.
* Monitoramento de desempenho: CloudWatch, X-Ray.

### Resumo:

Utilizar os recursos da AWS de forma eficiente para garantir alta performance.

### Definição em uma frase:

Otimizar o uso de recursos para fornecer alta performance e capacidade de resposta em cargas de trabalho.

### Definição em uma palavra:

Otimização.

### Palavras Chave da Eficiência de Desempenho:

Uso eficiente, otimização, escalabilidade, personalizar soluções, revisar e inovar, monitorar desempenho, compensações e contrabalanceamento, democratizar tecnologias avançadas, alcance global, arquitetura sem servidor, experimentar com mais frequência, seleção apropriada de recursos.

### Palavras-chave:

Escalabilidade, otimização, latência, throughput, caching.

## SEGURANÇA

### O que é?

A habilidade de proteger dados, sistemas e ativos para aproveitar as tecnologias de nuvem para melhorar sua segurança.

* **Foco Principal:** Proteger informações e sistemas, garantindo a confidencialidade, integridade e disponibilidade dos dados.
* **Âmbito:** Proteção de dados e sistemas.
* **Objetivo:** Garantir a confidencialidade, integridade e disponibilidade dos dados.
* **Métricas:** Número de incidentes de segurança, conformidade com políticas.
* **Uso prático:** Utilizar o AWS IAM para conceder permissões de acesso mínimas aos recursos da AWS, seguindo o princípio do menor privilégio.
* **Diferenças notáveis:** Prioriza a proteção de dados e sistemas contra acessos não autorizados e ameaças.

### Princípios de design de segurança

* Implementar uma base de identidade sólida
* Ativar rastreabilidade
* Aplicar a segurança em todas as camadas
* Automatizar
* Proteger dados em trânsito e repouso
* Manter as pessoas longe dos dados
* Preparar-se para eventos de segurança

### Práticas recomendadas de segurança

* Fundamentos de segurança
* IAM
* Detecção
* Proteção de infraestrutura
* Proteção de dados
* Resposta a incidentes
* Segurança das aplicações

### Conceitos Chave:

* Controle de acesso: AWS IAM.
* Criptografia: AWS KMS, ACM.
* Segurança de rede: VPC, WAF, Shield.
* Conformidade: AWS Config, GuardDuty.

### Resumo:

Proteger a infraestrutura e os dados contra acessos não autorizados e ameaças.

### Definição em uma frase:

Implementar medidas para proteger sistemas e dados contra acessos não autorizados e ameaças.

### Definição em uma palavra:

Proteção.

### Palavras Chave de Segurança:

Proteção, detecção, confidencialidade, integridade, disponibilidade, gerenciamento de permissões, controle e detecção de eventos, privilégio mínimo, rastreabilidade, captura de logs e métricas, segurança em camadas, proteger dados em trânsito e repouso, afastar pessoas dos dados, preparar para eventos de segurança, resposta a incidentes, IAM, criptografia, segurança de rede e conformidade.

## CONFIABILIDADE

### O que é?

Confiabilidade é a capacidade de uma carga de trabalho de executar sua função pretendida de forma correta e consistente durante um período de tempo esperado.

* **Foco Principal:** Capacidade de um sistema se recuperar de falhas e continuar funcionando.
* **Âmbito:** Continuidade dos negócios.
* **Objetivo:** Minimizar o tempo de inatividade e a perda de dados.
* **Métricas:** Tempo de inatividade, taxa de falhas, RTO/RPO.
* **Exemplo de uso:** Implementar uma arquitetura Multi-AZ para o Amazon RDS, garantindo alta disponibilidade do banco de dados em caso de falha de uma zona de disponibilidade.
* **Diferenças notáveis:** Visa garantir a resiliência e a recuperação de sistemas em caso de falhas, assegurando a continuidade.

### Princípios de design de Confiabilidade

* Recuperar-se automaticamente de falhas
* Testar os procedimentos de recuperação
* Dimensionar horizontalmente para aumentar a disponibilidade agregada da carga de trabalho
* Parar de adivinhar a capacidade
* Gerenciar alterações na automação

### Práticas recomendadas de confiabilidade

* Fundamentos
* Arquitetura de carga de trabalho
* Gerenciamento de alterações
* Gerenciamento de falhas

### Conceitos Chave:

* Redundância: Multi-AZ, regiões da AWS.
* Failover: Route 53, Elastic Load Balancing.
* Backups: AWS Backup, S3 Glacier.
* Recuperação de desastres: AWS DR.

### Resumo:

Garantir a disponibilidade e resiliência do sistema.

### Definição em uma frase:

Projetar sistemas que se recuperam de falhas e continuam funcionando de forma resiliente.

### Definição em uma palavra:

Resiliência.

### Palavras Chave:

Resiliência, recuperação de falhas, consistência de execução, adicionar ou remover recursos dinamicamente, mitigar interrupções, prever e impedir falhas, testar procedimentos de recuperação, escalar horizontalmente, gerenciar alterações, parar de adivinhar capacidade, gerenciamento de falhas, reparar automaticamente, cotas de serviços, redundância, failover, backup e recuperação de desastres.

## OTIMIZAÇÃO DE CUSTOS

### O que é?

É o processo de otimização para utilizar todos os recursos alcançando os resultados estabelecidos com menor preço possível e ainda atendendo aos requisitos funcionais.

### Princípios de design de otimização de custos

* Prática de gerenciamento financeiro na nuvem
* Adotar um modelo de consumo
* Avaliar a eficiência geral
* Parar de gastar dinheiro com trabalho pesado indiferenciado
* Analisar e atribuir despesas

### Práticas recomendadas de otimização de custos

* Prática de gerenciamento financeiro na nuvem
* Conscientização sobre despesas e uso
* Recursos econômicos
* Segmento de recurso de oferta e demanda
* Otimização ao longo do tempo

### Resumo:

Busca a eficiência financeira, minimizando gastos sem comprometer desempenho e segurança.

### Definição em uma frase:

Executar sistemas com o menor custo possível, sem comprometer desempenho e segurança.

### Definição em uma palavra:

Economia.

### Palavras Chave:

Gerenciamento de custos, economia, adotar modelo de consumo, otimizar ao longo do tempo, conscientização e reconhecimento de despesas, utilizar serviços gerenciados, transparência nos custos, analisar e atribuir despesas, relatórios de custos e uso, marcação de recursos, notificações de orçamentos, alertas de pagamento, desativação de recursos, granularidade por hora, selecionar recursos apropriados, adotar modelos de consumo, prever alteração de recursos, revisar regularmente, equiparar oferta com a demanda, medir eficiência geral.

## SUSTENTABILIDADE

### O que é?

Compreender os impactos dos serviços usados, quantificar os impactos durante todo o ciclo de vida da carga de trabalho e aplicar princípios de design e práticas recomendadas para reduzir esses impactos especialmente no consumo e na eficiência de energia.

* **Foco Principal:** Minimizar os impactos ambientais da infraestrutura de nuvem, otimizando o uso de recursos e reduzindo o consumo de energia.
* **Âmbito:** Responsabilidade ambiental e social das operações de nuvem.
* **Objetivo:** Reduzir a pegada de carbono, promover a eficiência energética e utilizar recursos de forma sustentável.
* **Métricas:** Consumo de energia, emissões de carbono, utilização de recursos renováveis, eficiência de recursos computacionais.
* **Exemplo de uso:** Utilizar instâncias EC2 otimizadas para energia, implementar práticas de desligamento automático de recursos ociosos e escolher regiões da AWS com alta utilização de energia renovável.
* **Diferenças notáveis:** Visa minimizar os impactos ambientais na nuvem, promovendo práticas sustentáveis e responsáveis.

### Princípios Sustentabilidade:

* Compreender seu impacto
* Estabelecer metas de sustentabilidade
* Maximizar a utilização
* Antecipar e adotar novas ofertas de hardware e software mais eficientes
* Usar serviços gerenciados
* Reduzir o impacto posterior

### Práticas recomendadas:

* Seleção de região
* Alinhamento à demanda
* Padrões de software e arquitetura
* Padrões de dados
* Hardware e serviços
* Processo e cultura

### Resumo:

Reduzir o impacto ambiental das operações de nuvem.

### Definição em uma frase:

Implementar práticas que minimizem o impacto ambiental da infraestrutura de nuvem.

### Definição em uma palavra:

Responsabilidade.

### Palavras Chave:

Sustentabilidade, impacto ambiental, eficiência energética, recursos renováveis, pegada de carbono, redução de consumo de energia, minimizar impactos ambientais, responsabilidade social, otimização de cargas de workloads, implantação de escalabilidade, eficiência de código, adoção de algoritmos modernos, dimensionamento adequado, redução de desperdício, redução de emissão de carbono, compreender o impacto dos serviços, energia renovável e a eficiência energética.

## FERRAMENTA ONLINE Well-Architected Framework

### O que é?

Well-Architected Framework é um mecanismo de aprimoramento contínuo que ajuda os clientes a avaliar consistentemente as cargas de trabalho em relação às práticas recomendadas da Amazon Web Services.

* Mecanismo = Medir - Aprimorar - Aprender (MAA)
* Componentes = Conteúdo, Ferramenta e Dados (CFD)
* Conteúdo = Pilares e Lentes, Princípios de Design, Práticas Recomendadas e Perguntas (PLPPP)

### Para que serve?

O WA-tool serve para analisar o estado das suas aplicações e cargas de trabalho, fornecendo um local central para as práticas recomendadas e orientações de arquitetura.

### Por que usar o Well-Architected Framework?

* Para criar e implantar com rapidez
* Para diminuir ou mitigar os riscos
* Para tomar decisões informadas
* Para conhecer as práticas recomendadas

### O que são Lentes Personalizadas?

As lentes são extensões da ferramenta Well Architected que fornecem orientação adicional e perguntas específicas para cargas de trabalho com características únicas.

Elas permitem uma análise mais profunda para cenários e setores específicos fornecendo recomendações mais direcionadas.

### Fluxo de trabalho de aprimoramento do Well-Architected

* Identificar riscos e oportunidades de aprimoramento
* Entender riscos e oportunidades de aprimoramento
* Determinar soluções prescritivas
* Priorizar aprimoramentos
* Implementar e acompanhar os aprimoramentos

### Quais são as novidades do AWS Well-Architected?

* Pilar de sustentabilidade adicionado à ferramenta do AWS Well-Architected
* AWS re:Post a partir da ferramenta do AWS Well-Architected




