# ⚙️ Casos de teste

## Módulo de Checkout ✅ 
---

### Id: CT-01  
**Título:** Preencher os dados do comprador com sucesso  

**Pré-condições:**  
Possuir um produto já adicionado no carrinho e estar na tela "Checkout: Your Information"  

**Passos:**  
1. Preencher o campo "First Name" com caracteres alfabéticos, incluindo acentuação (ex: "João")  
2. Preencher o campo "Last Name" com caracteres alfabéticos, incluindo acentuação (ex: "Batista Caçador")  
3. Preencher o campo "Postal Code" com um valor numérico válido  
4. Clicar no botão "Continue"  

**Resultado esperado:**  
O usuário deve ser encaminhado para a tela "Checkout: Overview", contendo os dados do produto, valores e informações de pagamento.  

---

### Id: CT-02  
**Título:** Validar campos obrigatórios não preenchidos  

**Pré-condições:**  
Possuir um produto já adicionado no carrinho e estar na tela "Checkout: Your Information"  

**Passos:**  
1. Manter o campo "First Name" vazio e preencher os outros campos obrigatórios  
2. Clicar no botão "Continue" e validar a mensagem de erro exibida  
3. Manter o campo "Last Name" vazio e preencher os outros campos obrigatórios  
4. Clicar no botão "Continue" e validar a mensagem de erro exibida  
5. Manter o campo "Postal Code" vazio e preencher os outros campos obrigatórios  
6. Clicar no botão "Continue" e validar a mensagem de erro exibida  

**Resultado esperado:**  
O sistema deve interromper o fluxo de checkout e exibir a mensagem solicitando o preenchimento obrigatório de cada campo específico.  

---

### Id: CT-03  
**Título:** Finalizar compra com sucesso  

**Pré-condições:**  
Possuir um produto já adicionado no carrinho, ter preenchido os dados do comprador e estar na tela "Checkout: Overview"  

**Passos:**  
1. Verificar os detalhes do produto exibido na tela de resumo do pedido  
2. Clicar no botão "Finish"  

**Resultado esperado:**  
O sistema deve redirecionar para a página "Checkout: Complete!" e exibir a mensagem confirmando que a compra foi concluída com sucesso.  

---

### Id: CT-04  
**Título:** Finalizar compra sem adicionar item no carrinho  

**Pré-condições:**  
Não possuir nenhum produto adicionado no carrinho e estar na tela "Your Cart"  

**Passos:**  
1. Acessar a página "Your Cart"  
2. Verificar se o carrinho está vazio  
3. Clicar no botão "Checkout"  

**Resultado esperado:**  
O sistema deve impedir o avanço no fluxo de checkout quando o carrinho estiver vazio, exibindo uma mensagem informando que é necessário adicionar produtos antes de prosseguir.  

---

### Id: CT-05  
**Título:** Cancelamento de checkout  

**Pré-condições:**  
Possuir um produto já adicionado no carrinho, ter preenchido os dados do comprador e estar na tela "Checkout: Overview"  

**Passos:**  
1. Clicar no botão "Cancel"  
2. Aguardar o redirecionamento da página  
3. Acessar a página "Your Cart"  

**Resultado esperado:**  
O sistema deve redirecionar para a página "Products" e o item adicionado anteriormente deve permanecer no carrinho.  

---

## Módulo do Carrinho 🛒 
---

### Id: CT-06  
**Título:** Adicionar item no carrinho pelo catálogo de produtos com sucesso  

**Pré-condições:**  
Estar na página "Products"  

**Passos:**  
1. Escolher qualquer produto do catálogo  
2. Clicar no botão "Add to Cart"  
3. Clicar no ícone do carrinho no menu de navegação  

**Resultado esperado:**  
O ícone do carrinho deve exibir a quantidade "1" e o carrinho deve conter o item adicionado, com todos os dados do produto válidos.  

---

### Id: CT-07  
**Título:** Remover item no carrinho pelo catálogo de produtos com sucesso  

**Pré-condições:**  
Estar na página "Products" e ter adicionado um produto pelo catálogo  

**Passos:**  
1. Escolher o item do catálogo que foi adicionado ao carrinho  
2. Clicar no botão "Remove"  
3. Clicar no ícone do carrinho no menu de navegação  

**Resultado esperado:**  
O ícone do carrinho deve voltar ao estado original, indicando que o carrinho está vazio. Na tela do carrinho, a lista de itens deve estar vazia.  

---

### Id: CT-08  
**Título:** Remover item no carrinho pela tela "Your Cart"  

**Pré-condições:**  
Possuir qualquer item adicionado ao carrinho  

**Passos:**  
1. Clicar no ícone do carrinho  
2. Selecionar o item que foi adicionado  
3. Clicar no botão "Remove"  

**Resultado esperado:**  
O carrinho deve ficar vazio e não deve ser possível prosseguir para checkout, exibindo apenas o botão "Continue Shopping".  

---

### Id: CT-09  
**Título:** Adicionar vários itens ao carrinho  

**Pré-condições:**  
Estar na página "Products"  

**Passos:**  
1. Escolher dois ou mais produtos do catálogo  
2. Clicar no botão "Add to cart"  
3. Clicar no ícone do carrinho no menu de navegação  

**Resultado esperado:**  
O ícone do carrinho deve indicar a quantidade de itens adicionados e o carrinho deve conter todos os dados dos produtos válidos.  

---

## Módulo de login 🔐  
---

### Id: CT-10  
**Título:** Realizar login com sucesso  

**Pré-condições:**  
Estar na página de login do Swag Labs e utilizar o nome de usuário "standard_user"  

**Passos:**  
1. Preencher o campo "Username" com o usuário pré-definido  
2. Preencher o campo "Password" com a senha válida exibida na seção "Password for all users"  
3. Clicar no botão "Login"  

**Resultado esperado:**  
O usuário deve conseguir logar com sucesso e ser direcionado para a tela "Products"  

---

### Id: CT-11  
**Título:** Tentar realizar login sem preencher o campo "Username"  

**Pré-condições:**  
Estar na página de login do Swag Labs  

**Passos:**  
1. Manter o campo "Username" vazio  
2. Preencher o campo "Password" com a senha válida exibida na seção "Password for all users"  
3. Clicar no botão "Login"  

**Resultado esperado:**  
O sistema deve impedir o login e a mensagem "Epic sadface: Username is required" deve ser exibida para o usuário  

---

### Id: CT-12  
**Título:** Tentar realizar login sem preencher o campo "Password"  

**Pré-condições:**  
Estar na página de login do Swag Labs e utilizar o nome de usuário "standard_user"  

**Passos:**  
1. Preencher o campo "Username" com o usuário pré-definido  
2. Manter o campo "Password" vazio  
3. Clicar no botão "Login"  

**Resultado esperado:**  
O sistema deve impedir o login e a mensagem "Epic sadface: Password is required" deve ser exibida para o usuário  

---

### Id: CT-13  
**Título:** Tentar realizar login com usuário inválido  

**Pré-condições:**  
Estar na página de login do Swag Labs  

**Passos:**  
1. Preencher o campo "Username" com um usuário que não esteja na lista "Accepted usernames are:" exibida na tela de login  
2. Preencher o campo "Password" com a senha válida exibida na seção "Password for all users"  
3. Clicar no botão "Login"  

**Resultado esperado:**  
O sistema deve impedir o login e a mensagem "Epic sadface: Username and password do not match any user in this service" deve ser exibida para o usuário  

---

### Id: CT-14  
**Título:** Tentar realizar login com senha inválida  

**Pré-condições:**  
Estar na página de login do Swag Labs e utilizar o nome de usuário "standard_user"  

**Passos:**  
1. Preencher o campo "Username" com o usuário pré-definido  
2. Preencher o campo "Password" com uma senha diferente da exibida na seção "Password for all users"  
3. Clicar no botão "Login"  

**Resultado esperado:**  
O sistema deve impedir o login e a mensagem "Epic sadface: Username and password do not match any user in this service" deve ser exibida para o usuário  

---

## Módulo do catálogo 🛍️  
---

### Id: CT-15  
**Título:** Validar o filtro de produtos por nome de A a Z (ordem alfabética)  

**Pré-condições:**  
Estar na tela de catálogo de produtos - "Products"  

**Passos:**  
1. Clicar na lista suspensa abaixo do menu de navegação (ícone de filtro)  
2. Escolher a opção "Name (A to Z)"  

**Resultado esperado:**  
O catálogo deve exibir os produtos organizados por nome em ordem alfabética crescente (A-Z)  

---

### Id: CT-16  
**Título:** Validar o filtro de produtos por nome de Z a A (ordem alfabética decrescente)  

**Pré-condições:**  
Estar na tela de catálogo de produtos - "Products"  

**Passos:**  
1. Clicar na lista suspensa abaixo do menu de navegação (ícone de filtro)  
2. Escolher a opção "Name (Z to A)"  

**Resultado esperado:**  
O catálogo deve exibir os produtos organizados por nome em ordem alfabética decrescente (Z-A)  

---

### Id: CT-17  
**Título:** Validar o filtro de produtos ordenados por preço (ordem crescente)  

**Pré-condições:**  
Estar na tela de catálogo de produtos - "Products"  

**Passos:**  
1. Clicar na lista suspensa abaixo do menu de navegação (ícone de filtro)  
2. Escolher a opção "Price (low to high)"  

**Resultado esperado:**  
O catálogo deve exibir os produtos organizados por preço em ordem crescente  

---

### Id: CT-18  
**Título:** Validar o filtro de produtos ordenados por preço (ordem decrescente)  

**Pré-condições:**  
Estar na tela de catálogo de produtos - "Products"  

**Passos:**  
1. Clicar na lista suspensa abaixo do menu de navegação (ícone de filtro)  
2. Escolher a opção "Price (high to low)"  

**Resultado esperado:**  
O catálogo deve exibir os produtos organizados por preço em ordem decrescente  

---

### Id: CT-19  
**Título:** Validar a tela de produto expandido  

**Pré-condições:**  
Estar na tela de catálogo de produtos - "Products"  

**Passos:**  
1. Escolher um produto do catálogo  
2. Clicar no produto escolhido  
3. Clicar na opção "Back to products", localizada na parte esquerda da tela, abaixo do menu de navegação  

**Resultado esperado:**  
O produto deve ser exibido de forma expandida, contendo todos os dados válidos e idênticos aos exibidos na tela de catálogo, em uma nova tela na mesma aba do navegador.  
A opção "Back to products" deve estar visível e clicável, e ao clicar, o usuário deve ser direcionado novamente para a tela "Products"  






