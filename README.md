# Wazuh

Wazuh es una plataforma de seguridad que proporicona medidas de prevención, detección y respuesta de de amnenazas, protegiendo las cargas de trabajo locales, en configuraciones virtualizadas, contenedores o la nube.

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