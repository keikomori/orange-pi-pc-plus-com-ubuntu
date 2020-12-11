<h6>Configuração</h6>
<h1 align="center">Acessando a Orange Pi via VScode</h1>
<h6 align="center">by Keiko</h6>

> É requisito ter acesso via SSH para seguir estes passos, mas olha que legal, já tenho aqui um tutorial pra te ajudar [Acesso via SSH](https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/edit/master/Acesso-via-SSH.md)

> Também é requisito ter o VS Code instalado, vou deixar o link aqui se for te ajudar [Instalação VS Code](https://code.visualstudio.com)

<h4>Vamos iniciar atualizando todas as dependências!</h4>

```
sudo apt-get update && apt-get upgrade -y
```

<h4>Primeiros passos</h4>

- Instalação da extensão: `Remote-SSH`

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh.jpg" alt="alt text" width="300"/>

- No canto esquerdo inferior do VS Code possui um botão, clique nele para aparecer as opções como as do exemplo abaixo

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-config.jpg" alt="alt text" width="300"/>

- Selecione: `Connect Host > Add New SSH Host`

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-inserir-ssh.jpg" alt="alt text" width="300"/>

> Insira o ssh keiko@<IP> -A

- Selecione a configuração:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-inserir-ssh-config.jpg" alt="alt text" width="300"/>

> Confirme se está tudo certo:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-inserir-ssh-config2.jpg" alt="alt text" width="300"/>

- Não podemos esquecer de inserir o PATH nas configurações do VS Code

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-add-path.jpg" alt="alt text" width="300"/>

- Novamente clique naquele botão no canto inferior esquerdo e selecione `Connect to Host`

- Selecione o Host que você configurou:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-inserir-ssh-config3.jpg" alt="alt text" width="300"/>

- Selecione a plataforma que esta utilizando, no nosso caso é o `linux`:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-seleciona-plataforma.jpg" alt="alt text" width="300"/>

- Será solicitada a senha:

<img src="https://github.com/keikomori/orange-pi-pc-plus-com-ubuntu/blob/master/img/extension-remote-ssh-insere-senha.jpg" alt="alt text" width="300"/>

Prontinho, você está conectado a Orange Pi via VS Code por meio do protocolo de segurança SSH :)






