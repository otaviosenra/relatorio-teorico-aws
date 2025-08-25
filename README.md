# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS 

Data: 2025-08-25 
Empresa: Abstergo Industries (Setor Farmacêutico citado no desafio solicitado pelo Bootcamp da DIO)  
Responsável: Otavio Senra

---

## Introdução 
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Otavio Senra.  
O objetivo do projeto foi elencar **3 serviços AWS com foco em otimização de custos**, mantendo a conformidade regulatória exigida pelo setor farmacêutico e garantindo escalabilidade para análise de dados e pesquisas clínicas.  

---

## Descrição do Projeto 
O projeto de implementação de ferramentas foi dividido em **3 etapas**, cada uma com objetivos específicos de redução de custos e melhoria operacional:  

### Etapa 1:  
- **Amazon S3 (com S3 Glacier para arquivamento)**  
- **Foco:** Armazenamento escalável e de baixo custo.  
- **Caso de uso:** Migração dos dados clínicos e relatórios de pesquisa para o S3 com políticas de ciclo de vida, movendo automaticamente dados antigos para S3 Glacier. Isso reduz custos de armazenamento em até 70% em comparação com soluções locais ou instâncias de armazenamento ativo.  

### Etapa 2:  
- **AWS EC2 + Auto Scaling (com instâncias Spot)**  
- **Foco:** Computação elástica e otimizada por demanda.  
- **Caso de uso:** Hospedagem de aplicações de análise de dados e simulação de pesquisas em instâncias EC2 configuradas com Auto Scaling. Para cargas de trabalho não críticas, foram usadas instâncias Spot, que podem gerar até 90% de economia em relação a instâncias On-Demand.  

### Etapa 3:  
- **Amazon RDS (com Aurora Serverless)**  
- **Foco:** Banco de dados relacional com pagamento conforme uso.  
- **Caso de uso:** Substituição da infraestrutura local de banco de dados por Amazon Aurora Serverless, garantindo alta disponibilidade e segurança. O modelo "serverless" permite que o banco seja dimensionado automaticamente de acordo com a carga, reduzindo custos em períodos de baixa utilização, comum em pesquisas que têm picos sazonais.  

---

## Conclusão 
A implementação de ferramentas na empresa **Abstergo Industries** possibilitou:  
- **Redução de custos imediata** em armazenamento, banco de dados e computação em nuvem.  
- **Maior escalabilidade** para suportar pesquisas clínicas e análises de dados.  
- **Conformidade regulatória** com padrões de segurança de dados exigidos pelo setor.  

Recomenda-se a continuidade da utilização dos serviços implementados e a avaliação de novos recursos da AWS, como **AWS Lambda** (para automação sem servidor) e **Amazon SageMaker** (para acelerar pesquisas com Machine Learning), visando ganhos adicionais em eficiência e inovação no setor farmacêutico.  
