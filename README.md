# Compartilhar LocalHost

## Instalação :desktop_computer:
* https://ngrok.com/download faça download do arquivo.zip
* Descompacte o arquivo.zip para um diretório conhecido

## Autenticação :shield:
* Cadastre-se na plataforma https://dashboard.ngrok.com/signup
* Entre em https://dashboard.ngrok.com/get-started/setup
* No dashboard, copie este código com a sua chave

<img src="https://github.com/pedrorivald/compartilhar-localhost/blob/main/img/autenticacao.png"/>

* Abra seu terminal
* Navegue até o local onde seu arquivo.zip foi descompactado
* Cole o comando copiado e aperte Enter 

<img src="https://github.com/pedrorivald/compartilhar-localhost/blob/main/img/autenticacao-terminal.png"/>

## Executar Ngrok :arrow_forward:
* No terminal e no mesmo diretório, digite:
```
  ./ngrok http 8080
```
* Trocando o 8080 pela sua porta
* Se tudo ocorrer bem basta copiar um dos links fornecidos ao executar e colar na URL de qualquer navegador
* Para fechar basta apertar as teclas CTRL + C

## Problemas ao executar
* Caso ./ngrok http 8080 não retornar nada
* Tente, trocando o 8080 pela sua porta:
```
./ngrok http 8080 -host-header="localhost:8080"
```
