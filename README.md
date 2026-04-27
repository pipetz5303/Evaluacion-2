# Evaluacion-2

Desarrollado por:

Felipe Castellanos Sánchez

Nicolás Romero Rozo

Parte 1:

Responda las preguntas de a continuación:

1. En el hacking ético en el campo del footprinting ¿Qué es el reconocimiento activo y cuál es el reconocimiento pasivo?

El reconocimiento activo es el proceso que se realiza a la infraestructura del cliente u objetivo con el fin de encontrar la mayor cantidad de información, esto con el riesgo de ser identificado por firewalls, o por otros sistemas de seguridad. Esta deteccion e incluso termino activo se debe a que es mas directa y precisa, ya que usa el escaneo de puertos con nmap el cual consulta todos los puetos abiertos (tambien cerrados y filtrados). 

Podría usarse el comando nmap -sn ip/rango para identeficar, no escanea.

El reconocimiento pasivo, al contrario del activo, evita la interaccion con el objetivo, se basa en buscar la informacion a traves de plataformas en bases de datos del gobierno, redes sociales y otras plataformas. Buscar en documentos, meta datos (puede que tengan usuarios). Y tambien realizar el comando nslookup o dig par identificar servidores y subdominios, que posteriormente puede intentar ver si estan desprotegidos.

2. ¿Qué son los exploits, payloads y post-exploits?, por favor dar dos ejemplos de los conceptos expuestos.

3. ¿Para que sirve metasploit y cómo lo puedo usar en entornos reales para la visualización de diferentes eventos anormales?

4. ¿Cúales son las diferencias entre la criptografía clásica, cuántica y post-cuántica?

5. ¿Qué es el blockchain?, ¿Para qué se utiliza actualmente en las criptomonedas?

6. ¿Qué protocolos y mecanismos de seguridad se usan en los sistemas biométricos de autenticación?

Parte 2:

Plantee una solución paso a paso de la situación descrita con lo aprendido en clase:

Bitcoin opera sobre una red descentralizada de nodos que ejecutan el software de referencia Bitcoin Core, cuyo código fuente se aloja en un repositorio público (GitHub). Tanto los nodos como el repositorio son blancos atractivos para adversarios: comprometer un nodo puede permitir robar fondos, realizar ataques de doble gasto o censurar transacciones; atacar el repositorio puede introducir vulnerabilidades en el propio protocolo (ataque a la cadena de suministro). Los estudiantes deberán aplicar una metodología de hacking ético completa (reconocimiento → escaneo → explotación → post-explotación) para identificar vectores de ataque realistas y diseñar contramedidas. 

Diseñar una estrategia de defensa integral (solución) que mitigue los riesgos identificados, aplicando la metodología de hacking ético en un entorno controlado de laboratorio.

Matriz de amenazas (vectores → impactos → probabilidad) específica para Bitcoin y su repositorio.

Informe sencillo que documente cada fase del hacking ético aplicado a lo visto en clase en un nodo Bitcoin simulado y al repositorio Bitcoin Core (revisar toda la documentación)

Parte 3:

Teniendo presente lo visto de blockchain y criptografía desarrollar lo siguiente:
Cree una cadena de bloques con una funcionalidad de mensajes entre dos servidores y explique el paso a paso y la funcionalidad. ¿Cómo se crea un bloque? ¿Qué tipo de encriptación se maneja en blockchain?




