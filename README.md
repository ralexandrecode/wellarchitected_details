# PRINCÍPIOS E DESIGN E PRÁTICAS RECOMENDADAS AWS WELL-ARCHITECTED

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
