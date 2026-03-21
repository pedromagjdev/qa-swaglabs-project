## 🐞 Bug Report

**ID:** BUG-01  
**Título:** Sistema permite finalizar checkout sem itens no carrinho  

---

**Ambiente:**  
- Sistema: Swag Labs - standard_user  
- URL: [https://www.saucedemo.com/](https://www.saucedemo.com/)  
- Navegador: Zen Browser 1.19.3b  
- Sistema Operacional: Windows 10 Home  

---

**Pré-condições:**  
- Estar logado com o usuário "standard_user"  

---

**Passos para reprodução:**  
1. Acessar a tela "Your Cart"  
2. Certificar que o carrinho está vazio  
3. Clicar no botão "Checkout"  
4. Observar que o sistema permite avançar para a tela "Checkout: Your Information"  
5. Preencher o formulário com dados válidos  
6. Clicar no botão "Continue"  
7. Na tela "Checkout: Overview", clicar no botão "Finish"  

---

**Resultado esperado:**  
O sistema deve impedir o avanço no fluxo de checkout quando o carrinho estiver vazio, exibindo uma mensagem informando que é necessário adicionar produtos antes de prosseguir.  

---

**Resultado obtido:**  
O sistema permite prosseguir com o checkout sem nenhum item no carrinho, além de permitir o preenchimento dos dados pessoais em "Checkout: Your Information" e a finalização da compra.  

---

**Severidade:** Alta  
**Prioridade:** Alta  

---

## Evidence:

### 📸 Screenshot - Checkout Overview
![Checkout Overview](./evidencias/checkout-overview.png)

### 📸 Screenshot - Checkout Complete
![Checkout Complete](./evidencias/checkout-complete.png)

### 🎥 Video
[Watch bug reproduction](link-do-seu-video)

---

**Impacto:**  
O usuário consegue finalizar uma compra sem itens no carrinho, comprometendo a lógica do sistema e as regras de negócio.
