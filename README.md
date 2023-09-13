# troca-botao-de-submissao-do-form
Script jQuery e Hook Ajax para substituir o botão de submissão de um formulário por outro que registre um usuário com função diferente do botão original de acordo com o valor inserido em um dos inputs.  (testes com WordPress em formulário do Ultimate Member)

## Onde colocar os códigos:
- O Script vai em um widget de HTML junto ao formulário.
- O Hook Ajax vai para "functions.php". Pode ser do tema, ou de preferência do tema filho.
Exemplo de rota: wwww/wp-content/nome-do-tema-filho/functions.php

## Observações:
- O SCRIPT adiciona um manipulador de eventos ao botão de submissão que impede o comportamento padrão do botão e, em vez disso, envia uma solicitação AJAX para registrar um novo usuário com outra função usando os valores dos campos de:
-- nome de usuário,
-- e-mail e
-- senha.

- Você precisará substituir submitButton, usernameField, emailField e passwordField pelos seletores apropriados para esses elementos em sua página.

- Além disso, você precisará adicionar o código AJAX ao arquivo functions.php do seu tema WordPress para registrar a ação AJAX que cria o novo usuário.

