
# 🧪 Plano de Testes — Assinaturas e Pagamentos Recorrentes

## 1. Objetivo

Definir cenários de teste para verificar a consistência entre planos de assinatura, ciclos de faturamento e autorizações de pagamentos recorrentes.

Este documento apresenta verificações baseadas na investigação e testes complementares propostos para um ambiente controlado.

## 2. Escopo

### Funcionalidades contempladas

- Criação de assinaturas.
- Validação de periodicidade.
- Geração de faturas.
- Associação entre pagamentos e assinaturas.
- Autorizações bancárias.
- Tratamento de pagamentos recusados.
- Cancelamento de recorrências.

### Fora do escopo

- Testes de carga e desempenho.
- Testes de invasão.
- Auditoria financeira ou contábil.
- Alterações diretas em sistemas de produção.

## 3. Matriz de cenários de teste

| ID | Cenário | Resultado esperado | Situação |
|---|---|---|---|
| CT-001 | Validar assinatura anual | Intervalo anual configurado | Verificado em casos selecionados |
| CT-002 | Validar próxima fatura | Renovação conforme ciclo anual | Verificado em casos selecionados |
| CT-003 | Relacionar pagamento e assinatura | Registros associados corretamente | Verificado em casos selecionados |
| CT-004 | Validar autorização bancária | Frequência compatível com o plano | Pendente |
| CT-005 | Verificar integração de recorrência | Configurações consistentes entre serviços | Pendente |
| CT-006 | Simular renovação anual | Cobrança conforme período contratado | Proposto |
| CT-007 | Simular pagamento recusado | Falha tratada conforme regra definida | Proposto |
| CT-008 | Cancelar autorização bancária | Ausência de novas cobranças não autorizadas | Proposto |

## 4. Casos de teste detalhados

### CT-001 — Validação da periodicidade anual

**Objetivo:** verificar se uma assinatura anual apresenta intervalo de faturamento compatível com o plano contratado.

**Pré-condições:**
- Existência de uma assinatura anual.
- Acesso autorizado aos detalhes da assinatura.

**Passos:**
1. Abrir os detalhes da assinatura.
2. Identificar o produto associado.
3. Verificar o intervalo de recorrência.
4. Conferir o período atual.

**Resultado esperado:** a assinatura deve apresentar recorrência anual.

**Situação:** verificado em casos selecionados por inspeção dos registros.

---

### CT-002 — Validação da próxima fatura

**Objetivo:** verificar se a próxima cobrança está programada para o ciclo de renovação contratado.

**Pré-condições:**
- Assinatura ativa.
- Informações de faturamento disponíveis.

**Passos:**
1. Acessar a assinatura.
2. Localizar a próxima fatura.
3. Conferir a data prevista.
4. Comparar com o intervalo contratado.

**Resultado esperado:** a próxima fatura deve respeitar a periodicidade anual.

**Situação:** verificado em casos selecionados por inspeção dos registros.

---

### CT-004 — Validação da autorização bancária

**Objetivo:** verificar se a autorização de pagamento automático corresponde à regra de negócio.

**Pré-condições:**
- Ambiente de teste disponível.
- Autorização de pagamento criada para teste.
- Acesso aos registros relevantes da integração.

**Passos propostos:**
1. Criar uma assinatura anual de teste.
2. Iniciar o fluxo de autorização bancária.
3. Verificar a frequência apresentada.
4. Comparar a autorização com o plano contratado.
5. Registrar eventuais divergências.

**Resultado esperado:** a autorização deve atender às regras de recorrência definidas para o produto e às condições do meio de pagamento.

**Situação:** pendente de validação técnica.

---

### CT-007 — Tratamento de pagamento recusado

**Objetivo:** verificar o comportamento do sistema quando uma tentativa de pagamento não é concluída.

**Pré-condições:**
- Ambiente de testes configurado.
- Método para simular falha de pagamento.

**Passos propostos:**
1. Iniciar uma tentativa de pagamento.
2. Simular uma recusa.
3. Verificar o status da transação.
4. Analisar o comportamento da assinatura.
5. Verificar mensagens e registros do sistema.

**Resultado esperado:** o sistema deve tratar a falha de acordo com as regras de negócio, sem registrar o pagamento como concluído.

**Situação:** teste proposto, não executado.

## 5. Critérios de aprovação

Um cenário poderá ser considerado aprovado quando:

- O resultado observado corresponder ao resultado esperado.
- Existirem evidências suficientes.
- Não houver divergências relevantes não justificadas.
- A execução e seu resultado estiverem documentados.

## 6. Registro de evidências

As evidências devem ser documentadas sem expor:

- Dados pessoais de clientes.
- Credenciais ou tokens.
- Identificadores internos.
- Informações financeiras confidenciais.
- Capturas de ambientes privados.

## 7. Limitações

Os cenários classificados como propostos não foram executados.

As verificações realizadas por inspeção de registros não equivalem a testes completos de integração ou simulações de cobranças futuras.

---

> Este plano foi desenvolvido para fins educacionais e de portfólio, com base em uma investigação prática anonimizada.
