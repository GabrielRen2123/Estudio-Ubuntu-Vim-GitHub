Auto-update:
	Es un programa programado en bash que ejecutara la actulizacion de linux y el auto borrado de archivos basura,
	los comandos que se llamaran y ejecutaran seran update, upgrade, clean, autoremove.
	
	update:
		El comando update buscara actulizaciones para el sistema y sus programas
	upgrade:
		Ejecutara las actulizaciones y las descargara
	clean:
		 limpia el repositorio local de archivos de paquetes recuperados
	autoremove:
		eliminara aquellos paquetes perdidos,
		generalmente paquetes de programas desinstalados, que ya no son necesarios.

Para abrir el script y ver que hace u en su caso modificarlo:
nano/vim/nvim auto-update | Solo funcionara si la terminal se encuentra en la misma carpeta que el archivo
	
Para instalar el comando se tiene que hacer el siguiente proceso:
(El archivo se llama auto-update)

	|control+alt+t : arbrir terminal y depues de eso|

	|cd <download> ó <descargas> ó <Carpeta donde yase el archivo>|

	|sudo mv auto-update /usr/bin/|

Para ejecutar el script se llamara como a un comando normal en la consola <auto-> y con tab se completara automaticamente el nombre.
El script puede recibir argumentos

	auto-update:
		Preguntara en cada fase si quiere descargar o borrar los archivos
	auto update -y:
		Instalara todas las actulizaciones sin preguntar pero se dentendra para el borrado de archivos basura y preguntara que hacer con ellos
	auto update -y -r ó -yr:
		no preguntara nada y hara todo el trabajo hasta mostrar el mensaje de que el equipo fue correctamente actualizado
