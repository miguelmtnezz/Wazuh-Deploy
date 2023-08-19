# Wazuh

Wazuh es una plataforma de seguridad que proporicona medidas de prevención, detección y respuesta de de amenazas, protegiendo las cargas de trabajo locales, en configuraciones virtualizadas, contenedores o la nube.

Los componentes que componen la solución de Wazuh son los siguientes:
- **Agente de Wazuh**: Prooporciona capacidades de prevenciçon, detección y respuesta cuando se instala en Endpoints como equipos portátiles, sobremesa, servidores, instancias en la nube o máquinas virtuales. Siendo compatible con SO actuales como, Windows, Linux, macOS, HP-UX, Solaris y AIX.
- **Servidor Wazuh**: Examina los datos recibidos de los agentes, procesandolos utilizando decodificadores y reglas para buscar indicadores de compromiso conocidos (IOC).
- **Elastick Stack**: Indexa y guarda las alertas del servidor Wazuh. Además, la integración de Wazuh junto a Kibana poroporciona una UX-UI para la visualizacion y análisis de datos.


## Requisitos previos

### SO Recomendado

El servidor Wazuh puede ser insalado en SO Linux x64, como:

| **Amazon Linux 2**                    	| **CentOS 7, 8**                       	|
|---------------------------------------	|---------------------------------------	|
| **Red Hat Enterprises Linux 7, 8, 9** 	| **Ubuntu 16.04, 18.04, 20.04, 22.04** 	|

### Hardware recomendado

El servidor Wazuh puede ser instalado en un unico nodo o en un cluster, sus requisitos son:

**Mínimo**

| RAM (GB) 	| CPU (Cores) 	|
|:--:|:--:|
| 2        	| 2           	|

**Recomendado**

| RAM (GB) 	| CPU (Cores) 	|
|:--:|:--:|
| 4        	| 8           	|

## Proceso de Instalación (Wazuh Server)

`#> sudo apt install curl `

`#> curl -sO https://packages.wazuh.com/4.3/wazuh-install.sh `

`#> sudo bash ./wazuh-install.sh -a`

Finalizado el proceso de instalación, hemos de guardar las credenciales ADMIN para poder hacer nuestro primer login/acceso.

Posteriormente realizado las ejecuciones de las anteriores ordenes descritas, se desplegara de manera automatizada todo su proceso de instalacion. Unicamente hemos de loguearnos al Dashboard web, abriendo un navegador e introducir la IP de la maquina que hemos instalado nuestro servidor.


## Proceso de Instalación (Wazuh Agent)

En este proceso de instalacion se ha vinculado como Agente un activo Windows 10 Pro.

Básicamente hemos de dirigirnos desde el dashborad, acceder a Wazuh > Agents y se desplegara un menu, donde hemos de seleccionar el SO de nuestra maquina que queremos escanear. Y seguir los pasos descritos en el propio portal web, para ser posteriormente ejecutados en el sistema final.