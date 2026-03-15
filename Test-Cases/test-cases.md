# ⚙️ Casos de teste
## Modulo de Checkout: 
---
Id: CT-01 <br>
Título: Preencher os dados do comprador com sucesso <br>
Pré-condições: Possuir um produto já adicionado no carrinho e estar na tela Checkout: Your Information" <br>
Passos: 
  1. Preencher o campo "First Name", com caracteres alfabéticos incluindo acentuação, exemplo: "João"
  2. Preencher o campo "Last Name", com caracteres alfabéticos incluindo acentuação, exemplo: "Batista Caçador"
  3. Preencher o campo "Postal Code", com um valor numérico válido.
  4. Clicar no botão continue <br>
Resultado esperado: O usuário deve ser encaminhado, para a tela: checkout: Overview, contendo os dados do produto, valores e informações de pagamento.  

Id: CT-02 <br>
Título: Validar campos obrigatorios não preenchidos <br>
Pré-condições: Possuir um produto já adicionado no carrinho e estar na tela "Checkout: Your Information" <br>
Passos: 
  1. Manter o campo "First Name" vázio e preencher os outros campos obrigatórios.
  2. Clicar no botão "Continue" e Validar mensagem de erro exibida
  3. Manter o campo "Last Name" vázio e preencher os outros campos obrigatórios"
  4. Clicar no botão "Continue" e Validar mensagem de erro exibida
  5. Manter o campo "Postal Code", vázio e preencher os outros campos obrigatórios.
  6. Clicar no botão Continue e validar mensagem de erro exibida <br>
Resultado esperado: O sistema deve interromper o fluxo de checkout e exibir a mensagem requerindo o preenchimento obrigatorio de cada campo especifico. 

Id: CT-03 <br>
Título: Finalizar compra com sucesso <br>
Pré-condições: Possuir um produto já adicionado no carrinho, ter preenchido os dados do comprador e estar na tela "Checkout: Overview" <br>
Passos: 
  1. Verificar os detalhes do produto exibido na tela de resumo do pedido
  2. Clicar no botão "Finish" <br>
Resultado esperado: O sistema deve redirecionar para a página "Checkout: Complete!" Deve ser exibida a mensagem confirmando que a compra foi concluída com sucesso

Id: CT-04 <br>
Título: Finalizar compra sem adicionar item no carrinho <br>
Pré-condições: Não possuir nenhum produto adicionado no carrinho e estar na tela "Your cart" <br>
Passos: 
1. Acessar a página "Your Cart"
2. Verificar se o carrinho está vazio
3. Clicar no botão "Checkout" <br>
Resultado esperado: O sistema deve impedir o avanço no fluxo de checkout quando o carrinho estiver vazio, exibindo uma mensagem informando que é necessário adicionar produtos antes de prosseguir.


Id: CT-05 <br>
Título: Cancelamento de checkout <br>
Pré-condições: Possuir um produto já adicionado no carrinho, ter preenchido os dados do comprador e estar na tela "Checkout: Overview" <br>
Passos: 
1. Clicar no botão "Cancel"
2. Aguardar redirecionamento da página
3. Acessar a página "Your Cart" <br>
Resultado esperado: O sistema deve redirecionar para a página "Products" e o item adicionado anteriormente, deve permanecer no carrinho. 

---



