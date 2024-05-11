# Projeto Imersão Alura - Chatbot de Inclusão Digital

<p align="center">
  <img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge" />
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlebard&logoColor=fff" />
</p>

## Introdução

O Imersão Alura é uma semana de aulas onde vamos criar um projeto do zero, com lives e discussões aprofundadas de tecnologia.

## O Projeto

O Projeto de Imersão Alura de Inteligência Artificial consiste em um Chatbot de Inclusão Digital. Nele, é possível que uma pessoa com deficiência visual possa realizar uma conversa direta com o Gemini através da API key do Google.

![api](https://github.com/Pesati/ImersaoAlura/assets/1533311/7f9f4d04-2b56-4934-8b7f-7007ddd09b73)


## Instalação

Foram utilizadas as bibliotecas abaixo para o funcionamento do projeto:

```bash
pip install time
pip install gtts
pip install soundfile
pip install sounddevice
pip install SpeechRecognition
pip install google.generativeai
pip install pyaudio // conda install -c anaconda pyaudio
```

Estas bibliotecas tem por finalidade:
-  Conectar com a API do Google;
-  Gravar o áudio do usuário;
-  Reproduzir o áudio do usuário;
-  Transformar o texto em áudio;
-  Transformar o áudio em texto;
-  Definir tempo de resposta.

## Etapas do projeto

- `Bibliotecas`: Realizar a importação das bibliotecas necessárias.
- `Variável de ambiente`: Criar um arquivo .env para salvar o código da API key gerada pela IA do Google no link: https://aistudio.google.com/app/apikey.
- `Modelo IA`: Configurar o modelo conforme a necessidade do usuário.
- `Microfone`: Habilitar o microfone do computador e compilar o código para que possar ser reproduzido e salvo o arquivo na pasta.
- `Texto em áudio`: Transformar o texto de retorno da IA em áudio para que o usuário possa ouvir a resposta do chatbot.
  
## Funcionamento

No final do código do projeto, tem a aba do Chatbot com a IA do Google. <br/> 
O usuário consegue interagir com o chat até solicitar para enviando um áudio para "encerrar" a conversa. <br />
A pasta de áudio tem os seguintes arquivos:
* fim.mp3 - Reproduz o áudio para o usuário informando como encerrar o chat.
* speech.mp3 - Cada resposta do chat a partir da pergunta do usuário, grava o arquivo de áudio para em seguida ser reproduzido.
* wait_user.mp3 - Reproduz um áudio no momento em que ele precisa falar alguma coisa para o chatbot.

## Autor

| [<img loading="lazy" src="https://avatars.githubusercontent.com/Pesati" width=115><br><sub>André Pesati Revoredo</sub>](https://github.com/Pesati) |
| :---: |
