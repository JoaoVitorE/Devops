PROJETO DE DEVOPS(MAQUINAS VIRTUAIS)

A aplicação Vagrant subirá duas maquinas, seu nomes seriam PHP e SQL sendo o PHP o Formulario onde puxará dados do GitHub e a SQL seria um banco de dados que subira
com suas configurações;

Utilize o comando no terminal : vagrant up SQL

-Ao final da inicialização da maquina salve o IP da maquina observado na segunda placa de rede da maquina

Ao final de subir a maquina SQL utilize o comando no terminal : vagrant up PHP

Maquina PHP

-Ao final da inicialização terá que acessar a maquina usando o comando : vagrant ssh PHP

--Ao acessar a maquina PHP utilize o comando : sudo nano /var/www/html/dadoscontroler.php

---Ao acessar o diretorio precisa-se colocar o IP do Banco de Dados (Maquina "SQL") nos campos "x.x.x.x" colocados no diretorio

----Saia do diretorio salvando-o utilizando o comando CTRL+X+Y

-----Ao sair utilize o camando : sudo systemctl restart apache2

------Este comando reinicializará o apache que seria a aplicação para publicar na WEB os dados, aplicando assim as alterações feitas no diretorio "dadoscontroler.php"

Com essa configuração poderá ja utilizar o formulario pegando o IP do mesmo localizado na segunda placa de rede da maquina e colando o mesmo na URL do seu navegador;
Com isso ja esta feita a conexão com o banco de dados.
