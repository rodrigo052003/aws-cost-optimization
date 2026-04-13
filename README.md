# Arquitetura da Solução – Otimização de Custos AWS

<img width="1216" height="451" alt="arquitetura-aws" src="https://github.com/user-attachments/assets/7e7766f4-4427-48db-b9b1-8f8cf34252d2" />

Este repositório foi criado para o desafio de projeto da Digital Innovation One (DIO), com foco em arquitetura de nuvem e práticas de FinOps utilizando a Amazon Web Services (AWS).

---

## Sobre o Projeto

O objetivo deste projeto é propor uma solução estratégica para a empresa fictícia **Abstergo Industries**, visando à redução imediata de custos operacionais sem comprometer a eficiência técnica.

A proposta demonstra como a transição de uma infraestrutura tradicional para uma arquitetura moderna, escalável e orientada a eventos pode impactar diretamente os custos mensais de uma organização.

---

## Arquitetura da Soluç

A arquitetura adotada é baseada em um modelo **serverless e orientado a eventos**, com o seguinte fluxo:

1. Usuários realizam requisições ou enviam dados
2. Eventos acionam funções no AWS Lambda
3. O AWS Lambda processa as informações sob demanda
4. Os dados são armazenados no Amazon S3
5. O S3 aplica automaticamente políticas de otimização com Intelligent-Tiering
6. O AWS Compute Optimizer analisa o uso da infraestrutura e recomenda melhorias

Essa abordagem elimina a necessidade de servidores em execução contínua, adotando o modelo **pay-as-you-go**.

---

## Serviços AWS Utilizados

### AWS Lambda
- Execução de código sob demanda (serverless)
- Elimina custos com servidores ociosos
- Escalabilidade automática

### Amazon S3 Intelligent-Tiering
- Armazenamento com movimentação automática entre camadas
- Redução de custos com dados pouco acessados
- Alta disponibilidade sem gerenciamento manual

### AWS Compute Optimizer
- Análise de uso com Machine Learning
- Identificação de recursos superdimensionados
- Recomendações para redução de custos

---

## Estrutura do Repositório

- `relatorio.md`: Documentação detalhada da implementação e casos de uso

---

## Como Visualizar o Relatório

Acesse o relatório completo no link abaixo:

🔗 **Visualizar Relatório de Implementação**

---

## Autor

**Rodrigo Silva da Luz**  
Estudante de Ciência da Computação (UFRPE)  
Entusiasta de Cloud Computing

---

## Considerações Finais

Este projeto demonstra como a adoção de serviços gerenciados e arquiteturas modernas pode gerar ganhos reais em eficiência operacional e redução de custos, aplicando conceitos de FinOps em ambientes cloud.
