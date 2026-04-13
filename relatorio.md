# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 12 de Abril de 2026
Empresa: Abstergo Industries 
Responsável: Rodrigo Silva da Luz

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Rodrigo Silva da Luz. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar a diminuição de custos operacionais imediatos e otimizar o uso de recursos em nuvem.

## Descrição do Projeto
A arquitetura proposta integra os serviços AWS de forma coordenada, onde o AWS Lambda atua como núcleo de processamento acionado por eventos de usuários, armazenando dados no Amazon S3 e utilizando recomendações do AWS Compute Optimizer para ajustes contínuos. Essa abordagem substitui o modelo tradicional baseado em instâncias EC2 24/7 por um modelo dinâmico, escalável e orientado à eficiência de custos. 

O projeto de implementação focou em transformar gastos fixos em variáveis e automatizar a economia de recursos. As etapas do projeto foram:

Etapa 1: 
- **Nome da ferramenta:** AWS Lambda
- **Foco da ferramenta:** Computação Serverless (sem servidor).
- **Descrição de caso de uso:** Substituição de servidores EC2 subutilizados que executavam tarefas agendadas. Com o Lambda, a empresa passa a ser tarifada apenas pelos milissegundos de execução do código, eliminando o custo de manter servidores ligados 24/7 sem necessidade.

Etapa 2: 
- **Nome da ferramenta:** Amazon S3 Intelligent-Tiering
- **Foco da ferramenta:** Gerenciamento automático de ciclo de vida de dados.
- **Descrição de caso de uso:** Implementação de uma camada de armazenamento inteligente que move automaticamente dados pouco acessados para classes de custo mais baixo (como o S3 Glacier). Isso reduz custos de backup e logs sem impactar a disponibilidade dos arquivos.

Etapa 3: 
- **Nome da ferramenta:** AWS Compute Optimizer
- **Foco da ferramenta:** Otimização de recursos baseada em Machine Learning.
- **Descrição de caso de uso:** Utilização da ferramenta para analisar o histórico de uso das instâncias e bancos de dados. O serviço identifica recursos "superdimensionados" e recomenda a redução para tipos de instâncias mais baratas que atendem à mesma demanda, evitando o desperdício de performance paga e não utilizada.

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado uma redução de custos estimada entre 20% e 35% no primeiro trimestre. Além da economia financeira, as soluções implementadas aumentam a escalabilidade e a eficiência operacional. Recomenda-se a continuidade do monitoramento através do AWS Cost Explorer e a revisão mensal das recomendações do Compute Optimizer.

## Anexos

1. Documentação de arquitetura Serverless.
2. Planilha de projeção de economia mensal (FinOps).
3. Guia de boas práticas para armazenamento no S3.

Assinatura do Responsável pelo Projeto:

Rodrigo Silva da Luz
