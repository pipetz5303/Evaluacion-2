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

Los tres conceptos hacen parte de los pasos que se deben realizar al momento de realizar un ataque informatico.

Los exploits se aprovechan de un error o bug ya sea en el sistema operativo, o en la aplicación. Una vez se identifica la vulnerabilidad, el exploit toma control. Por ejemplo los scripts que inyecion de SQLy otros programas que atacan vulnerbilidades en SMB como EternalBlue

El payload es el paso siguiente una vez se ingresa, es lo que exploit transporta y ejecuta cuando se ingresa al sistema. Un ejemplo puede ser el ransoware y reverse shell.

Post-Exploit son las acciones realizadas después de comprometer el sistema para mantener el acceso, escalar privilegios o extraer datos. como ejemplos podrian ser Mimikatz o la creación de un nuevo usuario con permisos de administrador ya que puedo ser root (comprobar con whoami). 

3. ¿Para que sirve metasploit y cómo lo puedo usar en entornos reales para la visualización de diferentes eventos anormales?

Metasploit sirve para encontrar, explorar y confirmar las vulnerabilidades que puede haber en un sistema o redes. Nos ayuda a verificar que tan protegido estamos y como podemos prevenir los ataques. Lo podemos usar para realizar escaneo ya sea de dispositivos, servicios y sistemas operativos de red. Aca reconcer algun dispositivo diferente o anormal no alerta. 

Adicional metasploit contiene diferentes base de datos con exploits para poder usarse, ingresar, escalar privilegiosm, realizar payloads para controlar diferentes opciones.

4. ¿Cúales son las diferencias entre la criptografía clásica, cuántica y post-cuántica?

Las diferencias son que la criptografia clasica, es la que usamos actualmente en la mayoria de nuestros sistemas, en especial internet. Utiliza  una serie de logaritmos, y numeros primos grantes que si un computador intenta resolverlos le tomaria miles de años, eso brinda cierta seguridad. Podriamos decir que aun es muy segura nuestro sistema actual clasico. 

Pero, abre la puerto a la criptografia cuantica, la cual ya usa leyes de fisica cuantica, y en especial el principio de incertidumbre de Heisenberg y el entrelazamiento cuantico. Al observar la clave, esa observacion altera el estado de las particulas, alterando el dato a tomar. Se seguridad es demasiado alta. 

Pensaria uno que la post-cuantica seria un paso mas adelante de la cuantica, en realidad es un proceso que busca que ni los equipos o computadores cuanticos, puedes descifrarlos porque generan formular que los costaria igual de años de realziar. Busca blindarse frente a algoritmos que son potentes con la criptografia de nuestros dias.

5. ¿Qué es el blockchain?, ¿Para qué se utiliza actualmente en las criptomonedas?

El blockchain es una cadena de bloques que esta descentralizado, lo que permite su seguridad. El blockchain se caracteriza porque cuando el dato se escribe en el bloque y la cadena, no puede ser modificado ni borrado . Como esta en varios nodods o computadores, se tienen copias del registro para controlar que no se cambie. Entonces su seguridad se basa en que añades una huella digital unica del bloque anterior a la cadena, si cambias algo en un bloque, la cadena cambiara y al no ser la misma cadena en el bloque 2, enviaria una alarma de fraude. Se utliza en las transacciones de criptomonedas por sus facilidades en transferencias, seguridad y validacion. Ya que no se necesita un banco que centralice la informacion porque todos los nodos tienen su cadena para verificar, lo que hace transparente y seguro.

6. ¿Qué protocolos y mecanismos de seguridad se usan en los sistemas biométricos de autenticación?

Existen varios como los mecanismos de proteccion de plantillas, no se guardan imagenes sino que se generan una plantilla con la informacion. Esta la biometria cancelable en caso de ser hackeada la base datos. Un mecanismo de seguridad es la deteccion de vitalidad para evitar dar accesos con fotos, mascaras 3D. El mecanismo analiza textutas, bordes, reflejos para saber si es tejido o imagenes adicionando por ejemplo movimientos al cuerpo como parpadear o acercarse.

El protocolo FIDO2 permite la autenticacion de la huella en el celular pero solo envia una firma digital del celular. Con eso la huella permanece en el celular sin salir por seguridad. Utilizan tambien protocolos de emparejamiento seguro para evitar en el medio. A nivel de hardware hay un mecanismo que es match-on-card donde la comparacion y verificacion de la huella se hace en el chip de sensor para que no se almacene en la RAM y pueda ser extraida.

Parte 2:

Plantee una solución paso a paso de la situación descrita con lo aprendido en clase:

Bitcoin opera sobre una red descentralizada de nodos que ejecutan el software de referencia Bitcoin Core, cuyo código fuente se aloja en un repositorio público (GitHub). Tanto los nodos como el repositorio son blancos atractivos para adversarios: comprometer un nodo puede permitir robar fondos, realizar ataques de doble gasto o censurar transacciones; atacar el repositorio puede introducir vulnerabilidades en el propio protocolo (ataque a la cadena de suministro). Los estudiantes deberán aplicar una metodología de hacking ético completa (reconocimiento → escaneo → explotación → post-explotación) para identificar vectores de ataque realistas y diseñar contramedidas. 

Diseñar una estrategia de defensa integral (solución) que mitigue los riesgos identificados, aplicando la metodología de hacking ético en un entorno controlado de laboratorio.

Matriz de amenazas (vectores → impactos → probabilidad) específica para Bitcoin y su repositorio.

Informe sencillo que documente cada fase del hacking ético aplicado a lo visto en clase en un nodo Bitcoin simulado y al repositorio Bitcoin Core (revisar toda la documentación)

Parte 3:

Teniendo presente lo visto de blockchain y criptografía desarrollar lo siguiente:
Cree una cadena de bloques con una funcionalidad de mensajes entre dos servidores y explique el paso a paso y la funcionalidad. ¿Cómo se crea un bloque? ¿Qué tipo de encriptación se maneja en blockchain?




