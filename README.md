# Servidor de Live Streaming com NGINX

Um servidor para live streaming simples, somente o essencial para você transmitir e assistir ✨

```
Esse projeto foi desenvolvido durante a gravação de um vídeo para o meu canal. Acesse o vídeo aqui: https://youtu.be/CrEzeBwLZPU 
```

## Requisitos 
- Docker 
- [Extensão para o chrome native MPEG-DASH + HLS Playback para o Chrome](https://chromewebstore.google.com/detail/native-mpeg-dash-+-hls-pl/cjfbmleiaobegagekpmlhmaadepdeedn) _(ou você também pode tocar o vídeo no safari se estiver usando um MacOS)_
- [OBS](https://obsproject.com/pt-br/download)

## Tecnologias
- Docker compose
- NGINX

## Protocolos 
- RTMP (Real Time Message Protocol)
- HLS (HTTP Live Streaming)

## Como executar

Suba os containers utilizando docker compose
```
docker-compose up --build
```

Abra o [OBS](https://obsproject.com/pt-br/download) > Configurações > Transmissão > Servidor
```
rtmp://localhost:1935/live
```
Clique em ok e depois clique em **Iniciar transmissão**

## Como assistir a transmissão
No chrome com a [ MPEG-DASH + HLS Playback](https://chromewebstore.google.com/detail/native-mpeg-dash-+-hls-pl/cjfbmleiaobegagekpmlhmaadepdeedn) ou no Safari acesse:
```
http://localhost:8081/live/.m3u8
```
