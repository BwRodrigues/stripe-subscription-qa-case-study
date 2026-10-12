
# 🔎 Auditoria de Assinaturas e Pagamentos Recorrentes

### Estudo de Caso | Quality Assurance (QA) | Stripe | Análise de Sistemas

![Status](https://img.shields.io/badge/Projeto-Documentado-22c55e)
![QA](https://img.shields.io/badge/Foco-Quality%20Assurance-2563eb)
![Tipo](https://img.shields.io/badge/Tipo-Estudo%20de%20Caso-8b5cf6)

---

## 📌 Sobre o projeto

Este repositório apresenta um estudo de caso técnico e anonimizado sobre a investigação de possíveis inconsistências em sistemas de assinaturas e pagamentos recorrentes.

O projeto demonstra a aplicação prática de conceitos de **Quality Assurance (QA)**, análise de sistemas, validação de regras de negócio e documentação técnica.

A investigação aborda a relação entre periodicidade de assinaturas, faturamento e autorizações bancárias.

> 🔐 **Confidencialidade:** este material não apresenta nomes de empresas, clientes, credenciais, valores ou identificadores internos. Os diagramas são conceituais e não representam arquiteturas reais de produção.

---

## 🎯 Objetivos

- Investigar comportamentos inesperados em pagamentos recorrentes.
- Validar a periodicidade de assinaturas.
- Analisar registros de pagamentos e faturas.
- Identificar riscos e possíveis inconsistências.
- Documentar resultados e limitações da investigação.
- Estruturar cenários e casos de teste de QA.

---

## 📚 Documentação técnica

| Documento | Descrição |
|---|---|
| [🐞 Cenário do problema](docs/01-cenario-do-problema.md) | Contexto, riscos e hipóteses investigadas |
| [🧪 Metodologia](docs/02-metodologia.md) | Processo de investigação e análise de evidências |
| [📊 Resultados](docs/03-resultados.md) | Comportamentos confirmados e pendências |
| [📋 Plano de testes](docs/04-plano-de-testes.md) | Matriz de cenários e casos de teste QA |
| [🏗️ Fluxograma](docs/05-fluxograma.md) | Fluxo conceitual e pontos de validação |

---

## 🛠️ Tecnologias e competências

| Tecnologia / Competência | Aplicação |
|---|---|
| Stripe | Análise de assinaturas, pagamentos e faturas |
| Quality Assurance | Investigação e validação de regras de negócio |
| APIs | Compreensão dos fluxos de integração |
| Análise de dados | Interpretação e classificação de registros |
| Git e GitHub | Versionamento e documentação |
| Markdown | Estruturação de documentação técnica |
| Mermaid | Representação visual de processos |

---

## 🔍 Principais aprendizados

A experiência reforçou que **a configuração correta de uma assinatura não garante, isoladamente, a consistência de todo o fluxo de pagamentos**.

Entre os aprendizados estão:

- Diferenciar evidências de hipóteses.
- Verificar regras de negócio em diferentes componentes.
- Identificar limitações nas informações disponíveis.
- Documentar resultados de maneira objetiva.
- Comunicar riscos e pendências à equipe técnica.

---

## ⚠️ Limitações

Este projeto documenta uma experiência de investigação e apresenta cenários de teste para estudo.

Não contém código de produção, integração funcional com APIs de pagamento ou testes automatizados.

Os cenários propostos não devem ser interpretados como testes efetivamente executados.

---

## 👨‍💻 Autor

**Brendow Rodrigues**

Estudante de Análise e Desenvolvimento de Sistemas, com foco em Quality Assurance, Python, APIs e integrações.

[LinkedIn](https://www.linkedin.com/in/dev-brendow-rodrigues/) | [GitHub](https://github.com/BwRodrigues)

---

⭐ Projeto desenvolvido para aprendizado e construção de portfólio profissional em Tecnologia da Informação.
