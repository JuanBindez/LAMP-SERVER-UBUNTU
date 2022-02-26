Como instalar o LAMP no Linux Ubuntu


Passo 1. Abra um terminal;
Passo 2. Dentro do terminal do Ubuntu, digite o comando abaixo (Observe que o símbolo ^ não é um erro, o comando é assim mesmo). Depois de digitar o comando, pressione a tecla “enter”, e quando for solicitado, digite a senha e a tecla “enter” novamente. Após a listagem dos pacotes necessários, será perguntado se deseja realmente continuar a instalação. Para confirmar, digite “S” e tecle “enter”;


~$ sudo apt-get install lamp-server^


###########################################################

Se quiser instalar uma ótima ferramenta de administração para o MySQL, use o comando abaixo;


~$ sudo apt-get install phpmyadmin



para testar o LAMP crie um arquivo com extensão .php e execute

~$ echo "<?php phpinfo(); ?>" | sudo tee /var/www/html/test.php




