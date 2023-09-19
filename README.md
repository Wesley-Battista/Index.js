# Index.js

Tutorial de como usar o arquivo node.js

1- instalar o Nodejs

a-)Abra o terminal de comandos (CTRL+ALT+T) e digite os comandos a seguir:

b-)sudo apt install python3-pip
Aguarde a instalação

c-)pip3 install --user nodeenv
Aguarde a instalação

d-)Teste a instalação com o comando nodeenv --version, caso dê erro, digite source ~/. profile ou reinicie a máquina e repita o comando de teste

2- Instalar com o Nodeenv

a-)Abra um terminal, selecione a pasta onde ficará a pasta que irá conter o NodeJs. Digite:

b-)nodeenv nodejs-env
Onde: nodeenv é o comando e nodejs-env é o nome da pasta (diretório) que irá ser
instalado o NodeJs

c-)Após a instalação para ativar esta versão do NodeJs, digite:
source ./nodejs-env/bin/activate

O indicador de prompt irá mudar, sinalizando que você está com o
ambiente ativo.

d-)Para testar digite:
node --version
Será informado a versão do NodeJs que está habilitada neste terminal

e-)Para desativar digite:
deactivate_node
O prompt irá sinalizar que o ambiente não está mais ativo

3- Criando o servidor Node.js

a-) Antes de começar, veja se o Node está desativado

b-) Vá para a pasta que você criou ao instalar o Node.js e crie um arquivo com extensão .js (um exemplo, index.js).

c-) Abra esse arquivo para editar seu conteúdo com o comando: sudo nano index.js

d-) Dentro dele coloque o código: 

var http = require('http');

http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end('Wesley Batista da Silva , 19/09/2023');
}).listen(8009);

e-) Salve o arquivo e ative o Node.

f-) Por fim, digite o seguinte endereço em um navegador: localhost:8009
