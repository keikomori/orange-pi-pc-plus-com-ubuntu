<h6>Instalação Orange Pi PC Plus</h6>
<h1 align="center">Orange Pi PC Plus com Ubuntu</h1>
<h6 align="center">by Keiko</h6>


<h4>Instalação do Armbian no Orange Pi PC Plus:</h4>

Vamos utilizar a versão **Bionic** que pode ser encontrada no [ORANGE PI PC PLUS ARMBIAN](https://www.armbian.com/orange-pi-pc-plus) essa é uma versão Ubuntu.

<img align="center" src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/bionic-armbian.jpg" alt="alt text" width="500"/>

<h4>Insira os dados solicitados</h4>

```
New root password: ********
Repeat password: ********

Creating a new user account. Press <Ctrl-C> to abort

Please provide a username (eg. your forename): <your-username>
Create password: ********
Repeat password: ********

Please provide your real name (eg. Keiko Mori): <your-name>
```

<h4>Configurando a conexão com Wi-Fi:</h4>

Utilize o seguinte comando:

```
root@orangepipcplus:~# nmtui-connect
```

Selecione a sua rede e insira a senha

<img align="center" src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/connect-wi-fi.jpg" alt="alt text" width="500"/>

<h4>Para utilizar a eMMC Flash como memória principal</h4>

```
root@orangepipcplus:~# nand-sata-install
```

Selecione a opçãp eMMC Flash, demorará alguns minutos para concluir, quando terminar finalize e desligue sua Orange Pi PC Plus da tomada e retire o cartão micro USB.

<h4>Mudando o horário/linguagem/hostname</h4>

```
root@orangepipcplus:~# armbian-config
```

Entre na opção Personal e configure o horário linguagem e hostname de acordo com sua necessidade

<h4>Atualize sua Orange Pi PC Plus</h4>

```
root@orangepipcplus:~# apt-get update && apt-get -y upgrade
```

<h4>Instalando a interface gráfica Ubuntu</h4>

```
root@orangepipcplus:~# apt-get install ubuntu-desktop --no-install-recommends -y
root@orangepipcplus:~# reboot
```

It's done!!

--------------------------------------------------------------------------

Tenho alguns tutoriais que podem lhe ajudar, caso queira é claro!

[Acesso a Orange Pi PC Plus via SSH](https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/Acesso-via-SSH.md)

[Acesso a Orange Pi PC Plus via VS Code](https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/Acesso-via-VScode.md)


Divirta-se!
