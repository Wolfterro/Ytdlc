## Ytdlc - Download de Vídeos e Músicas com youtube-dl

##### Descrição:

###### Este é um programa simples que permite o download de vídeos e músicas utilizando o programa [youtube-dl](https://github.com/rg3/youtube-dl).
###### Basta inserir o formato desejado e as ID's dos vídeos que deseja, não sendo necessária a URL inteira.
###### Possuo [scripts](https://github.com/Wolfterro/Youtube-DL-Script) que executam a mesma operação, mas decidi criar um programa em C ao invés disso.
###### É necessário possuir o youtube-dl instalado e reconhecido como comando interno para que o programa funcione!
###### Também é necessário possuir o programa [ffmpeg](https://www.ffmpeg.org/) ou libav-tools instalado para que o programa possa converter o vídeo para o formato desejado.
###### O programa é bem simples e pode ser utilizado com os seguintes comandos:

      Comandos:
      '-h' ou '--help':             Mostra esta tela de ajuda
      '-u' ou '--update':           Atualiza o youtube-dl
      '-v' ou '--version':          Mostra a versão deste programa
      
      Formatos:
      '--mp3':                      Converte o vídeo para o formato MP3
      '--wav':                      Converte o vídeo para o formato WAV
      
      '--mp4':                      Converte o vídeo para o formato MP4.
      '--webm':                     Converte o vídeo para o formato WEBM.
      '--mp4-conv':                 Converte o vídeo para o formato MP4 (conversão).
      '--webm-conv':                Converte o vídeo para o formato WEBM (conversão).

##### Download:

###### Você pode baixar o programa já compilado (x64) e executá-lo com o comando abaixo:

      wget 'https://raw.github.com/Wolfterro/Ytdlc/master/ytdlc'
      chmod +x ytdlc
      ./ytdlc [Formato] [ID do vídeo] ...

###### Você também poderá compilar o programa em seu sistema através do comando abaixo (é necessário possuir o GCC):

      wget 'https://raw.github.com/Wolfterro/Ytdlc/master/src/ytdlc.c'
      gcc ytdlc.c -o ytdlc
      ./ytdlc [Formato] [ID do vídeo] ...

###### Existe também a versão para Windows, e você pode baixá-lo já compilado (x86) clicando [aqui!](https://raw.github.com/Wolfterro/Ytdlc/master/Win/bin/ytdlc.exe)

###### Observação: Alguns anti-virus podem acusar o programa compilado para Windows como um possível Trojan. 
###### Para evitar este problema e também assegurar de que não tenho intenção de disseminar qualquer tipo de vírus, recomendo fortemente que utilize o [MinGW](http://www.mingw.org/) para compilar o programa em seu computador. Você poderá utilizar os comandos abaixo (requer o MinGW):

      windres ytdlc.rc -O coff -o ytdlc.res
      mingw32-gcc -o ytdlc.exe ytdlc.c ytdlc.res
      ytdlc [Formato] [ID do vídeo] ...

<br />
