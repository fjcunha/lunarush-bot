# Sobre:
Este bot tem o seu código aberto, de forma que qualquer pessoa pode vê-lo, fazer uma fork, ou updates.

Desenvolvi esse bot primeiramente para conseguir ter uma noite de sono 😴🥱 sem precisar ficar acordando de madrugada para dar start nas lutas. Eu decidi publica-lo aqui para ajudar o pessoal que como eu tem 3 guerreiras ou menos (podendo ter upgrades futuros para quem tem mais personagens).
Se este projeto conseguir salvar algumas horas de sono para você também, salva a grana da coca-cola 🥤
 
### Paypal:
[Donate:](https://www.paypal.com/donate/?business=HTKSK9AAKTRPQ&no_recurring=0&item_name=Just+another+computer+guy+looking+for+his+place+in+the+sun%2C+so+grateful+for+your+support.%0A%0AObrigado+pelo+apoio&currency_code=BRL)
https://www.paypal.com/donate/?business=HTKSK9AAKTRPQ&no_recurring=0&item_name=Just+another+computer+guy+looking+for+his+place+in+the+sun%2C+so+grateful+for+your+support.%0A%0AObrigado+pelo+apoio&currency_code=BRL

### Smart Chain Wallet(BUSD/BNB/LUS):
#### 0x0141D5033068E05427e4cAf840ecF06d12c926D2

## Aviso:

#### O uso e aplicação deste projeto é de sua total responsabilidade, Não me responsabilizo por eventuais penalidades sofridas por quem usar o bot, use por sua própria conta e risco.

# Instalação:
### Baixe e instale o Python pelo [site](https://www.python.org/downloads/) ou pela [windows store](https://www.microsoft.com/p/python-37/9nj46sx7x90p?activetab=pivot:overviewtab).

Se você baixar pelo site é importante marcar a opção para adicionar o
python ao PATH:
![Check Add python to PATH](https://github.com/fjcunha/lunarush-bot/blob/master/readme-images/path.png)

### Realize o download do codigo no formato zip, e extraia o arquivo.

### Copie o caminho até a pasta do bot:

![caminho](https://github.com/fjcunha/lunarush-bot/blob/master/readme-images/address.png)

### Abra o terminal.

Aperte a tecla do windows + r e digite "cmd":

![launch terminal](https://github.com/fjcunha/lunarush-bot/blob/master/readme-images/cmd.png)

### Navegue até a pasta do bot:
Digite o comando "cd" + caminho que você copiou:

![cd](https://github.com/fjcunha/lunarush-bot/blob/master/readme-images/cd.png)

### Instale as dependências:

```
pip install -r requirements.txt
```

  
![pip](https://github.com/fjcunha/lunarush-bot/blob/master/readme-images/pip.png)

### Pronto! Agora é só iniciar o bot com o comando

```
python3 index.py
```

![run](https://github.com/fjcunha/lunarush-bot/blob/master/readme-images/run.png)


# Como usar?

Abra o terminal, se ainda não tiver navegado para a pasta do bot dê novamente o comando

```
"cd" + caminho que você copiou
```

Para iniciar use o comando 

```
python3 index.py
```

Assim que ele iniciar ele vai começar tentando iniciar uma luta. Para que ele funcione é preciso que a janela do game esteja aparecendo na sua tela, e suas guerreiras já selecionadas nos 3 slots.
Ele vai constantemente checar se você foi desconectado para realizar o login novamente.

  ----------------

## Como funciona?

O bot não interage diretamente com o jogo, ele somente tira print da tela do
game para encontrar os botões e simula movimentos do mouse, isso faz com que
diferenciar o bot de um humano seja muito difícil.

## Ajustando o bot

### Por que uns ajustes podem ser necessários?

O bot usa reconhecimento de imagem para tomar decisões e movimentar o mouse e
clicar nos lugares certos. 
Ele realiza isso comparando uma imagem de exemplo com um screenshot da tela do
computador.
Este método está sujeito a inconsistências devido a diferenças na resolução da
sua tela e de como o jogo é renderizado no seu computador comparado com o
meu(o que usei para pegar as imagens exemplo).
É provável que o bot não funcione 100% logo de cara, e que você precise fazer
alguns ajustes aqui ou ali.

### Quais sao os problemas?

**Falso negativo** - O bot deveria reconhecer uma imagem, por exemplo, o botão de
mandar para trabalhar, mas não reconheceu a imagem na screenshot.

**Falso positivo** - O bot pensa que reconheceu a imagem que está procurando em um
lugar em que esta imagem não aparece.

Aqui tem uma [lista](#alguns-comportamentos-que-podem-indicar-um-falso-positivo-ou-negativo) de alguns problemas que podem ser ocasionados por falsos
positivos e negativos.

Para resolver estes problemas existem duas possibilidades, a regulagem do
parâmetro “threshold” no arquivo config.yaml ou a substituição da imagem de
exemplo na pasta “targets” para uma tirada no seu próprio computador:

  ### Threshold na config

  O parâmetro “threshold” regula o quanto o bot precisa estar confiante para
  considerar que encontrou a imagem que está procurando.
  Este valor de 0 a 1 (0% a 100%).
  Ex:

  Um threshold de 0.1 é muito baixo, ele vai considerar que encontrou a imagem
  que esta procurando em lugares que ela não está aparecendo ( falso positivo ).
  O comportamento mais comum pra esse problema é o bot clicando em lugares
  aleatórios pela tela. 


  Um threshold de 0.99 ou 1 é muito alto, ele não vai encontrar a imagem que
  está procurando, mesmo quando ela estiver aparecendo na tela. O comportamento
  mais comum é ele simplesmente não mover o cursor para lugar nenhum, ou travar
  no meio de um processo, como o de login.

  ### Substituição da imagem na pasta targets

  As imagens exemplo são armazenadas na pasta “targets”. Estas imagens foram
  tiradas no meu computador e podem estar um pouco diferente da que aparece no
  seu. Para substituir alguma imagem que não esta sendo reconhecida
  propriamente, simplesmente encontre a imagem correspondente na pasta targets,
  tire um screenshot da mesma área e substitua a imagem anterior. É importante
  que a substituta tenha o mesmo nome, incluindo o .png.


### Algumas configuraçoes podem ser mudadas no arquivo config.yaml, nao se esqueça de reiniciar o bot caso mude as configuraçoes.

## Curtiu? Dê aquela fortalecida :)

### Wallet:
#### 0xbd06182D8360FB7AC1B05e871e56c76372510dDf
### Paypal:
[Donate](https://www.paypal.com/donate/?business=HTKSK9AAKTRPQ&no_recurring=0&item_name=Just+another+computer+guy+looking+for+his+place+in+the+sun%2C+so+grateful+for+your+support.%0A%0AObrigado+pelo+apoio&currency_code=BRL)

