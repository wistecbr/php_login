# PHP Login

## Atividade

1) Crie um repositório no GitHub com nome php_login.
2) Crie uma página de formulário, contendo login e senha.
3) O formulário da página de login irá enviar os dados para a própria página usando o metodo post.
4) vocês deverão tratar os dados recebidos do metodo post, a senha deverá ser criptografada nesse momento.

* **OBS.:** Devido a proteção de dados, vamos precisar utilizar uma função para criptografar a senha, para isso vamos utilizar a criptogrfia MD5, php já possui uma função para isso;
https://www.php.net/manual/pt_BR/function.md5.php

5) Agora vamos verificar se o login e a senha são de fato os dados esperados. 
crie uma variavél $loginOficial = 'admin' $passOficial = '21232f297a57a5a743894a0e4a801fc3'
o $passOficial é a palavra 'admin' em md5 pode ser verificado no site (https://www.md5hashgenerator.com/)

6) Na verificação se o login e senha forem iguais ao esperado, redirecione o usuário para uma outra pagina de boas vindas, para redirecionar use a função disponivel na referência (https://www.php.net/manual/pt_BR/function.header.php)

* Caso o login não seja como esperado redirecione o usuário para a propria pagina de login, adicionando os seguintes caracteres '?login=erro'
ex.: se sua página de login está salva como login.php o seu location será '/login.php?login=erro'

7) Aqui iremos verificar o metodo GET, semelhante ao que fazemos com o post, porém usando a variavel $_GET, verifique se existe e se ela possui a propriedade login $_GET['login'] e se essa propriedade é igual a 'erro', caso seja iremos adicionar um elemento na tela informando ao usuário que houve erro no login.


## Para testar em sua máquina

1) Ir até a pasta do Xampp e renomear a pasta htdocs para ex.: htdocs.old2
2) criar nova pasta Htdocs
3) dentro dessa pasta colocar os arquivos do novo projeto.
