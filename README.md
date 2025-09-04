# RELATORIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

- Data: 02/09/2025
- Empresa: Abstergo Industries
- Responsável: Anita Lassala Leme da Silva

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa **Abstergo Industries**, realizado por **Anita Lassala Leme da Silva**. 
O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

### Etapa 1: **Otimização de Armazenamento com Amazon S3 Lifecycle Policies**

- *Nome da ferramenta:* Amazon S3 (Simple Storage Service) e S3 Lifecycle Policies.

- *Foco da ferramenta:*  Otimizar custos de armazenamento de dados não acessados frequentemente.

- *Descrição de caso de uso:* A Abstergo Industries armazena grandes volumes de dados históricos, backups e logs no Amazon S3. A análise de uso revelou que muitos desses arquivos eram acessados apenas esporadicamente, mas estavam armazenados em classes de armazenamento de custo mais alto (como o S3 Standard). A implementação de S3 Lifecycle Policies permitiu a transição automática desses dados para classes de armazenamento mais baratas, como S3 Standard-Infrequent Access (para dados acessados raramente) e S3 Glacier Deep Archive (para dados de longo prazo que precisam ser retidos por regulamentação, mas que são acessados em meses ou anos). Essa automação garante a redução contínua de custos sem a necessidade de intervenção manual.

### Etapa 2: **Gerenciamento e Redução de Custos de Computação com AWS EC2 Reserved Instances**

- *Nome da ferramenta:* Amazon EC2 (Elastic Compute Cloud) e EC2 Reserved Instances (RIs).

- *Foco da ferramenta:* Reduzir custos de instâncias de computação (servidores virtuais) que funcionam 24/7.

- *Descrição de caso de uso:* A Abstergo Industries utiliza várias instâncias EC2 para hospedar suas aplicações e serviços principais. Muitas dessas instâncias operam ininterruptamente para garantir a disponibilidade. Ao invés de pagar pelo modelo de "pay-as-you-go" (Sob Demanda), que é mais caro, foi realizada uma análise de uso e compromisso de utilização para a compra de EC2 Reserved Instances (RIs) com contrato de 1 a 3 anos. Isso garantiu um desconto significativo sobre o custo das instâncias, com uma economia de até 72% em comparação com o modelo sob demanda, para as instâncias que estão sempre em uso.

### Etapa 3: Análise e Otimização com AWS Cost Explorer

- *Nome da ferramenta:* AWS Cost Explorer.

- *Foco da ferramenta:* Visibilidade e controle sobre os gastos na nuvem.

- *Descrição de caso de uso:* Inicialmente, a Abstergo Industries tinha dificuldade em visualizar e atribuir custos a departamentos ou projetos específicos. A implementação e o uso regular do AWS Cost Explorer permitiram uma análise detalhada dos gastos. Por meio da criação de relatórios personalizados, foi possível identificar rapidamente os serviços mais caros, analisar tendências de gasto ao longo do tempo e até mesmo rastrear a economia gerada pelas ações das etapas 1 e 2. Além disso, o Cost Explorer ajudou a identificar recursos não utilizados ou subutilizados, como volumes de EBS (Elastic Block Store) desanexados e instâncias EC2 ociosas, permitindo sua exclusão para uma redução adicional de custos.

## Conclusão

A implementação de ferramentas na empresa Abstergo Industries tem como esperado a **diminuição imediata dos custos de infraestrutura de TI**, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

[Planilha de Controle de Gastos Mensais](https://docs.google.com/spreadsheets/d/1Cti9Gpfp-GxIWwJ38iW-AhvNh7lKNH9ouUNNZmtM9zo/edit?gid=1882383970#gid=1882383970)

Assinatura do Responsável pelo Projeto:

Anita Lassala Leme da Silva
