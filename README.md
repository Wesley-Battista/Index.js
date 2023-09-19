# Index.js

Tutorial de como usar o arquivo node.js

1- instalar o Nodejs

Abra o terminal de comandos (CTRL+ALT+T) e digite os comandos a seguir:
sudo apt install python3-pip
Aguarde a instalação
pip3 install --user nodeenv
Aguarde a instalação
Teste a instalação com o comando nodeenv --version, caso dê erro, digite source ~/. profile ou reinicie a máquina e repita o comando de teste

2- Instalar com o Nodeenv

Abra um terminal, selecione a pasta onde ficará a pasta que irá conter o NodeJs.
Digite:
nodeenv nodejs-env
Onde: nodeenv é o comando e nodejs-env é o nome da pasta (diretório) que irá ser
instalado o NodeJs
Após a instalação para ativar esta versão do NodeJs, digite:
source ./nodejs-env/bin/activate
O indicador de prompt irá mudar, sinalizando que você está com o
ambiente ativo.
Para testar digite:
node --version
Será informado a versão do NodeJs que está habilitada neste terminal
Para desativar digite:
deactivate_node
O prompt irá sinalizar que o ambiente não está mais ativo

3- Testar a instalação do Nodejs com o NodeEnv

Para testar instale o Node-Red, digitando:
npm install -g node-red
Aguarde a instalação do Node-Red
Após instalar, ative o Node-red, digitando:
node-red
