# Honeypot en AWS y análisis con Wazuh

En este proyecto desplegué un honeypot en AWS para observar y analizar la actividad real que recibe un servidor expuesto a Internet.

Utilicé Cowrie para simular un servicio SSH y Nginx para publicar la web de un banco ficticio, Aegis Bank. Los registros se centralizaron en un servidor Wazuh local, conectado mediante WireGuard.

## Trabajo realizado

- Integración de los registros y creación de una regla personalizada para Cowrie.
- Análisis de accesos SSH, comandos y transferencias de archivos.
- Investigación de escaneos e intentos de explotación web.
- Consulta de hashes de las muestras capturadas en VirusTotal, sin ejecutarlas.
- Creación de un dashboard para visualizar la actividad.

Durante el análisis se observaron búsquedas de archivos sensibles, escaneos automatizados y transferencias de ejecutables con detecciones relacionadas con troyanos y minería de criptomonedas. También se reconstruyeron sesiones para seguir los intentos de ejecución dentro del entorno simulado.

**Tecnologías:** AWS · Ubuntu Server · Cowrie · Nginx · Wazuh · WireGuard · VirusTotal

## Documentación

La memoria incluye la configuración, el análisis de los casos y las capturas de las evidencias.

📄 [Ver la memoria completa en PDF](honeypot-analisis-wazuh.pdf)
