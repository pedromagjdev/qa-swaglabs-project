# ⚙️ Casos de teste
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
  6. Clicar no botão Continue e validar mensagem de erro exibida
Resultado esperado: O sistema deve interromper o fluxo de checkout e exibir a mensagem requerindo o preenchimento obrigatorio de cada campo especifico. 

Id: CT-03
