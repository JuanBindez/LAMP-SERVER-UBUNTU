### Como instalar o LAMP no Linux Ubuntu


Passo 1. Abra um terminal;
Passo 2. Dentro do terminal do Ubuntu, digite o comando abaixo (Observe que o símbolo ^ não é um erro, o comando é assim mesmo). Depois de digitar o comando, pressione a tecla “enter”, e quando for solicitado, digite a senha e a tecla “enter” novamente. Após a listagem dos pacotes necessários, será perguntado se deseja realmente continuar a instalação. Para confirmar, digite “S” e tecle “enter”;


`~$ sudo apt-get install lamp-server^`

### agora deve autorizar a pasta www com O chmod

`~$ sudo chmod -R 777 /var/www`

### para ver o status do apache e mysql:

`~$ sudo systemctl status apache2`

`~$ sudo systemctl status mysql`

### para startar caso o serviço estiver inoperante:

`~$ sudo systemctl start apache2`

`~$ sudo systemctl start mysql`

### para reiniciar o serviço:

`~$ sudo systemctl restart apache2`

`~$ sudo systemctl restart mysql`





### ____________________________________________

### Se quiser instalar uma ótima ferramenta de administração para o MySQL, use o comando abaixo;


`~$ sudo apt-get install phpmyadmin`



### para testar o LAMP crie um arquivo com extensão .php

`~$ echo "<?php phpinfo(); ?>" | sudo tee /var/www/html/test.php`

### Reinicie o servidor apache digitando o comando abaixo e depois tecle “enter”;

`~$ sudo /etc/init.d/apache2 restart`
### ou
`~$ sudo systemctl restart apache2`

### Abra seu navegador favorito e na barra de endereço dele digite “http://localhost/test.php” (sem as aspas) e depois tecle “enter”. Serão mostradas todas as informações sobre a versão do PHP, MySQL e Apache que foram instalados.

![testephp](https://user-images.githubusercontent.com/79322362/155844567-f744faaf-fa46-4013-a4dd-903dec6e89b1.png)
