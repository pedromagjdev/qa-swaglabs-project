# 📄 Plano de Teste – Swag Labs

## 1. Objetivo

Garantir a qualidade das principais funcionalidades da aplicação **Swag Labs**, com foco no fluxo de compra (checkout), assegurando que o usuário consiga realizar a jornada completa de compra sem falhas críticas que impactem a receita do negócio.

---

## 2. Escopo

### 2.1 Dentro do Escopo

Serão realizados testes manuais funcionais nos seguintes módulos:

- Login
- Catálogo de Produtos
- Carrinho
- Checkout

Também serão executados testes de regressão básicos após correções de defeitos identificados.

---

### 2.2 Fora do Escopo

Não fazem parte deste ciclo de testes:

- Testes de Segurança
- Testes de Performance
- Testes de Usabilidade
- Testes de Acessibilidade
- Testes de Responsividade
- Testes automatizados

---

## 3. Itens a Serem Testados (Ordem de Prioridade)

1. Checkout
2. Carrinho
3. Login
4. Catálogo de Produtos

A priorização foi definida com base no impacto direto na receita e na jornada de compra do usuário.

---

## 4. Estratégia de Teste

Serão realizados testes manuais funcionais e testes de regressão utilizando as seguintes técnicas de teste:

- Particionamento de Equivalência
- Análise de Valor Limite
- Tabela de Decisão
- Transição de Estados
- Testes Exploratórios

Os testes serão executados diretamente na interface da aplicação (Front-end).

---

## 5. Critérios de Entrada

Os testes poderão ser iniciados quando:

- A aplicação estiver disponível para acesso.
- O ambiente estiver estável.
- As funcionalidades principais estiverem implementadas.
- Os requisitos mínimos estiverem definidos.

---

## 6. Critérios de Saída

Os testes serão considerados finalizados quando:

- Todos os casos de teste planejados forem executados.
- Não houver defeitos críticos ou bloqueadores em aberto.
- Os resultados forem devidamente documentados.
- Os defeitos identificados estiverem registrados.

---

## 7. Riscos Identificados

- Falhas críticas no fluxo de checkout podem gerar prejuízo financeiro direto.
- Erros no carrinho podem impedir a finalização da compra.
- Problemas de autenticação podem bloquear o acesso de usuários.
- Instabilidade do sistema pode comprometer a experiência do cliente.
- Riscos de segurança e indisponibilidade do sistema (fora do escopo deste ciclo).

---

## 8. Ferramentas Utilizadas

- Navegador Web (Chrome)
- GitHub para versionamento
- Documentação em Markdown

---

## 9. Tipo de Teste

- Teste Funcional Manual
- Teste de Regressão
- Teste Exploratório
