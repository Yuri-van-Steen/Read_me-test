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

![image](https://github.com/user-attachments/assets/715920c5-6075-4ed4-b9b1-a3467c0b410c)


Vale ressaltar, que essa API não contém somente os 176 jogos do banco de dados, mas sim uma gama muito maior de opções, por isso devemos retornar erro caso um jogo que não está listado no nosso banco de dados seja requisitado
