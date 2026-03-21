## 🐞 Bug Report

**ID:** BUG-01  
**Título:** Sistema permite conclusão de checkout sem itens adicionados ao carrinho

---

**Ambiente:**  
- Sistema: Swag Labs - standard_user  
- URL: [https://www.saucedemo.com/](https://www.saucedemo.com/) 
- Navegador: Zen browser 1.19.3b  
- Sistema Operacional: Windows 10 home  

---

**Pré-condições:**  
- Estar logado com o usuário standard_user

---

**Passos para reprodução:**  
1. Acesse a tela "Your Cart"  
2. Certifique se não possui nenhum item adicionado ao carrinho
3. Clique no botão "Checkout"
4. Prencha o formulário Checkout: Your Information com dados válidos
5. Clique no botão "Continue"
6. Na tela "Checkout: Overview" finalize a compra clicando no botão "Finish"

---

**Resultado esperado:**  

O sistema deve impedir o avanço no fluxo de checkout quando o carrinho estiver vazio, exibindo uma mensagem informando que é necessário adicionar produtos antes de prosseguir.

---

**Resultado obtido:**  

O sistema permite prosseguir com o checkout sem nenhum item no carrinho, além de permitir o preenchimento dos dados pessoais em "Checkout: Your Information" e a finalização do checkout. 

---

**Severidade:** Alta  
**Prioridade:** Alta  

---

**Evidência:**  
[Print, vídeo ou descrição detalhada do erro]  

