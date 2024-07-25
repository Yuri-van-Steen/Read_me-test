## O que contém no banco de dados

O banco de dados trabalhado e disponibilizado pelo [kaggle](https://www.kaggle.com) no seguinte link: (https://www.kaggle.com/datasets/codefantasy/list-of-bestselling-pc-games/data) contém uma lista dos 176 vídeo jogos mais vendidos na história. Organizado segundo as seguintes colunas (os nomes entre aspas são uma explicação ou tradução):

-  Game *"o nome do jogo"*
-  Total copies sold *"total de cópias vendidads"*
-  Series *"Se o jogo pertence a uma série de jogos e qual"*
-  Release date *"Data de lançamento do jogo"*
-  Genre(s) *"Gênero(s) do jogo"*
-  Developer(s) *"O studio/time desenvolvedor do jogo"*
-  Publisher(s) *"A companhia publicadora do jogo"*


A consulta de informações do banco de dados, portanto, pode ser realizada por qualquer um dos parâmetros apresentados. No entanto, no desenvolvimento do site, decidiu-se útil para o nosso caso a consulta por base no nome do jogo e o(s) gênero(s) ao qual ele pertence.

## A API de imagens

Além da leitura das informações do banco de dados de jogos, também utilizamos uma API que, pelo nome do jogo, retorna uma imagem de uma capa do jogo no formato 16:9.
Vale ressaltar, que essa API não contém somente os 176 jogos do banco de dados, mas sim uma gama muito maior de opções, por isso devemos retornar erro caso um jogo que não está listado no nosso banco de dados seja requisitado

![image](https://github.com/user-attachments/assets/ed69d392-d391-408c-a776-5d0839c4c5e5)


## Conexão com o MongoDB

O banco de dados é trabalhado por meio do MongoDB, um programa de database orientado à documentos, o qual utiliza documentos em JSON, schemas e consiste de um sistema NoSQL, ou seja, não necessariamente é relacional

Para se conectar ao MongoDB da Síntese Júnior, de início é necessário criar uma conta no MongoDB com seu e-mail síntese e enviar seu e-mail a um dos diretores em Projetos.
Em seguida, é necessário adicionar o IPV4 do computador sendo utilizado, para tal, no canto inferior esquerdo se encontra o menu "Network Access".
![image](https://github.com/user-attachments/assets/f3917102-8aee-40ed-8aab-d7a8cf4e1080)

Ao clicar, abre-se a página da lista de IPs de acesso.
Clique em "**ADD CURRENT IP ADRESS**"
![image](https://github.com/user-attachments/assets/23bb570d-90d7-4655-96f5-aa5c96e5ae79)

E pronto! O seu IP já está cadastrado no MongoDB para acesso à rede.

No entanto, caso haja algum erro pode-se configurar o IP manualmente.
Para encontrar o seu IP manualmente abra o terminal de seu computador e digite o seguinte comando segundo o seu sistema operacional: 

-  Windows: ipconfig /all
-  MacOS: ipconfig getifaddr en0
-  Linux: ip a

Procure pela opção de IPV4 caso apareça diversas opções.
Agora que você tem seu IP em mãos, volte a página no MongoDB e clique em "**Add IP Adress**" e por fim, digite seu IPV4 no primeiro campo.
Por fim, conclua a adição.
