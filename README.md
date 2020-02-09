# CSBase2020
A server-executable for the game "Counter-Strike 1.6" but updated to 2020.
Un servidor-ejecutable para el juego "Counter-Strike 1.6" pero actualizada al 2020.

Guide in English and Spanish
Guía en Español e Ingles

Solamente sistemas operativos Linux, probado únicamente en Ubuntu pero debería de funcionar en CentOS y Debian igualmente.
Only S.O Linux, tested only in Ubuntu, but it should be working on CentOS and Debian as same.

/////////// English \\\\\\\\\\\

How to install it?

Simply use "wget https://github.com/Drakunovu/CSBase2020/master.zip"
And after of that unzip the "master.zip"
Go into the folder "CSBase2020-master"
And then you have it, the Base 2020 for CS

How to execute it?

Go to the folder "cstrike" into the "CSBase2020-master" folder
Edit with a text editor the files "server.cfg" and "game.cfg"
These files comes in Spanish by default, change the hostname, rcon password and everything you want.

Open a screen with: "screen -S CSBase2020"
You can change the "CSBase2020" to a name you prefer onto the Screen
Open the server with: "./hlds_run -game cstrike -ip 127.0.0.1 -port 27015 -pingboost 3"
You can change as always the IP and the Port

And then you have it, the server is running now.
If for some reason, you can not enter the server, check your Firewall, IP and Port

Optional:
Delete the file "master.zip"
You can rename the folder "CSBase2020-master"

/////////// Spanish \\\\\\\\\\\

¿Cómo instalarlo?

Simplemente usa "wget https://github.com/Drakunovu/CSBase2020/master.zip"
Después de eso extrae el "master.zip"
Entra a la carpeta "CSBase2020-master"
Y ahí lo tienes, la Base 2020 para el CS

¿Cómo ejecutarlo?

Ve a la carpeta "cstrike" dentro de la carpeta "CSBase2020-master"
Edita con un editor de texto los archivos "server.cfg" y "game.cfg"
Estos archivos vienen en Español por defecto, cambia el hostname, rcon password y todo lo que tu quieras.

Abre una pantalla con: "screen -S "CSBase2020"
Puedes cambiar el "CSBase2020" a un nombre que tu prefieras para la Pantalla
Abre el servidor con: "./hlds_run -game cstrike -ip 127.0.0.1 -port 27015 -pingboost 3"
Como siempre, puedes cambiar la IP y Puerto.

Y ahí lo tienes, el servidor está ejecutandose ahora.
Sí por alguna razón no puedes entrar al servidor verifica tu Firewall, IP y Puerto

Opcional:
Borra el archivo "master.zip"
Puedes renombrar la carpeta "CSBase2020-master"
