
# 🔎 Auditoria de Assinaturas e Pagamentos Recorrentes

### Estudo de Caso | Quality Assurance (QA) | Stripe | Integrações

## 📌 Sobre o projeto

Este repositório apresenta um estudo de caso técnico e anonimizado, baseado em uma experiência prática de investigação de possíveis inconsistências em sistemas de pagamentos recorrentes.

O objetivo é demonstrar a aplicação de conceitos de Quality Assurance (QA), análise de sistemas, validação de regras de negócio e documentação técnica.

O estudo aborda a relação entre assinaturas, periodicidade de faturamento e autorizações de pagamentos automáticos.

## 🎯 Objetivos

- Investigar possíveis divergências entre assinaturas e autorizações de pagamento.
- Verificar a periodicidade de cobranças recorrentes.
- Analisar informações de assinaturas, faturas e transações.
- Identificar riscos e comportamentos inesperados.
- Documentar evidências e comunicar resultados técnicos.
- Desenvolver habilidades práticas relacionadas a QA e análise de sistemas.

## 🔐 Confidencialidade

Este estudo utiliza descrições genéricas e não apresenta dados de clientes, informações financeiras internas, credenciais ou identificadores de sistemas.

Os exemplos e diagramas apresentados têm finalidade exclusivamente educacional e demonstrativa.


---

## 🐞 Cenário do problema

### Contexto

Durante a análise de um sistema de assinaturas digitais, foi identificada uma possível divergência entre a periodicidade de faturamento configurada na plataforma de pagamentos e a frequência apresentada nas autorizações bancárias.

O modelo de negócio analisado utilizava assinaturas anuais, enquanto determinadas autorizações de pagamento automático apresentavam frequência mensal.

Essa diferença levantou dúvidas sobre o comportamento do fluxo de cobrança e a necessidade de verificar se as configurações estavam consistentes.

### ⚠️ Risco identificado

Uma divergência entre a periodicidade contratada e a autorização bancária pode gerar:

- Confusão para o cliente sobre futuras cobranças.
- Dúvidas sobre a recorrência dos pagamentos.
- Necessidade de revisão das configurações de integração.
- Riscos operacionais e de experiência do usuário.

**Importante:** a apresentação de uma autorização mensal não comprova, por si só, que uma cobrança mensal será executada.

### 🔍 Hipóteses de investigação

Foram consideradas as seguintes possibilidades:

1. A assinatura poderia estar configurada com periodicidade incorreta.
2. O sistema poderia apresentar divergência entre o plano contratado e o ciclo de faturamento.
3. A autorização bancária poderia utilizar uma periodicidade diferente da assinatura.
4. A integração entre os serviços de pagamento poderia exigir validação adicional.

As hipóteses foram utilizadas para orientar a análise, sem serem tratadas como causas comprovadas.


---

## 🧪 Metodologia de investigação

A investigação foi conduzida por meio da análise de informações disponíveis na plataforma de pagamentos, com foco na consistência entre assinaturas, transações e regras de negócio.

### 1. Levantamento de informações

Inicialmente, foram examinados os registros de assinaturas e pagamentos para compreender o comportamento do sistema.

As principais informações consideradas foram:

- Status das assinaturas.
- Produtos e planos associados.
- Valores e periodicidade de faturamento.
- Datas de início e renovação.
- Histórico de transações.
- Situação dos pagamentos.

### 2. Análise de transações

As transações foram classificadas de acordo com seus respectivos status:

- Pagamentos bem-sucedidos.
- Pagamentos cancelados.
- Pagamentos reembolsados.

Essa classificação permitiu diferenciar tentativas de pagamento de transações efetivamente concluídas.

### 3. Validação das assinaturas

Foram examinadas assinaturas relacionadas a pagamentos concluídos, verificando:

- Plano contratado.
- Intervalo de recorrência.
- Próxima data de faturamento.
- Valor previsto para renovação.
- Relação entre assinatura, pagamento e fatura.

O objetivo foi verificar se o ciclo de faturamento registrado correspondia à regra de negócio esperada.

### 4. Análise de inconsistências

As informações obtidas foram comparadas com as evidências de autorizações bancárias.

A investigação considerou que a periodicidade de uma assinatura e a frequência de uma autorização de pagamento são informações distintas.

Por esse motivo, a validação do faturamento não foi considerada suficiente para confirmar a configuração das autorizações bancárias.

### 5. Documentação e comunicação

Os resultados foram organizados e comunicados à equipe técnica responsável pela integração.

A documentação distinguiu:

- Comportamentos confirmados.
- Possíveis inconsistências.
- Hipóteses ainda não verificadas.
- Pontos que exigiam investigação adicional.

### 🛠️ Ferramentas e conhecimentos aplicados

- Stripe Dashboard.
- Análise de assinaturas e faturas.
- Histórico de transações.
- Interpretação de registros de API.
- Validação de regras de negócio.
- Investigação de problemas.
- Documentação técnica.
- Comunicação com desenvolvedores.

> Este estudo apresenta atividades de análise e investigação. Não representa a implementação de uma integração de pagamentos ou a execução de testes automatizados.


