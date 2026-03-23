# 📄 Plano de Teste – Swag Labs

## 1. Objetivo

Garantir a qualidade das principais funcionalidades da aplicação **Swag Labs**, com foco no fluxo de compra (checkout), validando que o usuário consiga realizar a jornada completa sem falhas críticas que impactem a experiência ou a conversão.

---

## 2. Escopo

### 2.1 Dentro do Escopo

Serão realizados testes manuais funcionais nos seguintes módulos:

* Login
* Catálogo de Produtos
* Carrinho
* Checkout

Também serão executados testes de regressão básicos após identificação de defeitos.

---

### 2.2 Fora do Escopo

Não fazem parte deste ciclo:

* Testes de Performance
* Testes de Segurança
* Testes de Acessibilidade
* Testes de Responsividade
* Testes automatizados

---

## 3. Prioridade dos Testes

1. Checkout
2. Carrinho
3. Login
4. Catálogo de Produtos

A priorização foi definida com base no impacto direto na jornada de compra e no negócio.

---

## 4. Estratégia de Teste

Os testes serão realizados manualmente na interface da aplicação, com foco em:

* Validação dos fluxos principais (happy path)
* Identificação de comportamentos inesperados
* Testes negativos (ações inválidas ou fora do fluxo esperado)
* Testes exploratórios para descoberta de falhas

Os cenários foram definidos com base na experiência do usuário e nas regras de negócio da aplicação.

---

## 5. Critérios de Entrada

Os testes iniciam quando:

* A aplicação estiver disponível
* O ambiente estiver estável
* As funcionalidades principais estiverem acessíveis

---

## 6. Critérios de Saída

Os testes são finalizados quando:

* Todos os cenários planejados forem executados
* Não houver defeitos críticos abertos
* Os resultados estiverem documentados

---

## 7. Riscos

* Falhas no checkout podem impactar diretamente a conversão
* Problemas no carrinho podem impedir a finalização da compra
* Erros no login podem bloquear o acesso do usuário

---

## 8. Ferramentas

* Navegador Web
* GitHub
* Documentação em Markdown

---

## 9. Tipos de Teste

* Teste Funcional Manual
* Teste de Regressão
* Teste Exploratório
