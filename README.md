# CSBase2020
Una base del juego Counter-Strike 1.6 actualizada a 2020

ADVERTENCIA: Si no usas Linux no uses esto, ya que es solo para Linux

# Contenidos

A medida que salgan nuevas versiones de ReHLDS y demás se ira actualizando.

ReHLDS v3.7.0.698

ReGameDLL v5.18.0.473

ReAPI v5.15.0.199

Reunion v0.1.0.133

AMXX v1.8.2

~~VoiceTranscoder v2017RC4~~

Revoice 0.1.0.34

SafeNameAndChat 1.1

# ¿Cómo usar?

Sencillo, basta con descargar el .zip o hacerle git clone al repositorio y por siguiente seguir las instrucciones:

1) Ejecutar el siguiente comando dependiendo si estás en Debian, Ubuntu o en otra distribución:

## CentOS:

yum clean all

yum update -y

yum upgrade -y

yum install glibc.i686 libstdc++.i686 -y

## Debian o Ubuntu

apt -y update

apt -y upgrade

apt -y install lib32gcc1

RECOMENDABLE NO USAR EL USUARIO 'root' PARA EJECUTAR EL SERVIDOR.

2) Entrar a la carpeta cstrike y modificar server.cfg y game.cfg a tu gusto.

3) Instalar tus plugins o lo que sea que quieras

4) Iniciar el servidor con el siguiente comando: "./hlds_run -game cstrike -map de_dust2 -port 27015", de esta manera se usa la IP especificada, el puerto especificado y con eso basta.

4.1) Cambiar variables necesarias, "-map" y "-port".

### Este README.md será actualizado pronto, estará solamente los contenidos y lo demás en la Wiki.
