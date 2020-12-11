<h6>Configuração</h6>
<h1 align="center">Acessando a Orange Pi via SSH</h1>
<h6 align="center">by Keiko</h6>


<h4>Vamos iniciar atualizando todas as dependências!</h4>

```
sudo apt-get update && apt-get upgrade -y
```

<h4>Necessitamos criar as chaves de acesso privada(computador) e pública(Orange Pi PC Plus)</h4>

- Para criar as chaves utilizaremos o [PUTTYgen](https://www.puttygen.com/), deixo aqui o link para instalação caso não tenha na sua máquina.

- Instalado o PUTTYgen gere uma chave, vai aparecer uma imagem como a que segue abaixo:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/puttygen-generate.jpg" alt="alt text" width="300"/>

> Isso vai levar um tempo, então pode ir lá passar seu cafezinho tranquilamente.

- Após finalizar a criação das chaves, crie uma pasta chamada `.ssh` em seu computador e salve nesta pasta as chaves criadas, vou te mostrar um exemplo:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/puttygen-chaves.jpg" alt="alt text" width="300"/>

> Essa área destacada em vermelho é que será utilizada para inserir na Orange Pi

> Utilizando os botões `save public key` e `save private key` salve-as na pasta `.ssh` que foi criada no seu computador.

<h4>Utilizando o PUTTY que você já instalou vamos acessar nossa Orange Pi PC Plus</h4>

> Você vai precisar saber o IP que a Orange Pi está utilizando, vou deixar aqui um programa legal para descobrir caso você tenha dificuldades [Advanced IP Scanner](https://www.advanced-ip-scanner.com/br/)

- Insira o IP da sua Orange Pi

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/putty-inserirIP.jpg" alt="alt text" width="300"/>

Será solicitado o login e a senha configurada quando você instalou o SO na sua Orange Pi e teremos uma tela parecida com essa:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/putty-acesso.jpg" alt="alt text" width="300"/>

- Agora vamos criar uma pasta dentro da Orange Pi e chamá-la de `.ssh` e acessá-la com o seguinte comando:

```
mkdir .ssh && cd .ssh
```

- Agora vamos criar um arquivo para salvar a chave criada com o PUTTYgen

```
nano authorized_keys
```

- Cole a chave criada e salve o arquivo, se nunca utilizou o editor de texto `nano` vou te dar uma dica:

`<Ctrl+o> : para salvar`

`<Ctrl+x> : para sair`

> Agora sua chave já está na sua Orange Pi PC Plus

- Para finalizar esta parte no seu computador acesse `~/.ssh/id_rsa.ppk`, e clique para que a chave seja executada na sua máquina permitindo que e comunique com a chave pública existente na Orange Pi
