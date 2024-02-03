# Unidad 1 - Introducción, conceptos básicos y capa física

El primer invento similar a lo que conocemos hoy en día como redes de
comunicación fue la del telégrafo. Luego, le siguió la del teléfono, y ambos
tenían una cualidad que persistió hasta aproximadamente la década del 70: la
**conmutación de circuitos**.

La conmutación de circuitos como indica el nombre implicaba que haya operarios
encargados de conectar a las dos personas / aparatos que querían iniciar una
comunicación (cof cof, *operadora, comuníqueme con pirulito*)

Este approach tiene varias desventajas, por lo que mayoritariamente entre los
años 1959-1969 se desarrollaron las ideas que nos llevaron a la **conmutación
de paquetes**, cuyo objetivo principal era resultar en una red más tolerante a
fallas. Cómo se logró esto?

- Redundancia: que haya múltiples caminos entre dos puntos de la red
- Descentralizada: toleracia a censura
- División en fragmentos de los mensajes cosa de que puedan tomar caminos
  diferentes.

*ARPANET* (Advanced Research Projects Agency Network) fue uno de los más importantes.

## Estandarización

Las tecnologías de redes con conmutación de paquetes se suiguieron
desarrollando, terminando a mediados de los 80 con una situación en la que
tenías muchas redes distintas cada una con su implementación particular y sus
propios detalles. Se empieza a hablar de la idea de tener una red única (en
mayo de 1983 ISO publica “ISO 7498:The Basic Reference Model for Open Systems
Interconnection” como un estándar internacional)

![Diagrama Modelo OSI](./img/osi_model.png)

El modelo OSI describe tódo lo que sucede con la información en una
comunicación entre dos puntos. Parte el proceso en 7 capas, en la que cada una
tiene un fin particular y cuyas entidades relevantes son definidas por eso. Por
ejemplo, en la capa de aplicación tu entidad puede ser un archivo mientras que
en la capa de de red tu entidad puede ser el paquete.

Si bien se usa el modelo OSI para estudiar teoría de comunicaciones, hoy en día
el verdadero ganador fue el modelo de TCP/IP, en donde hay 4 capas en lugar de
las 7 que propone OSI

![Diferencias OSI vs TCP/IP](./osi_tcp_differences.png)

```admonish info title="[osi the internet that wasnt](https://spectrum.ieee.org/osi-the-internet-that-wasnt)"
TLDR: OSI y TCP/IP compitieron durante un tiempo, pero una de las mayores
diferencias radicaba en que OSI era un protocolo que se estaba gestando por un
comité conformado por gente de la industria y cada uno quería tener su
influencia sobre el protocolo. Esto resultó en problemas para ponerse de
acuerdo y en un modelo que si bien era completo era mucho más difícil de
implementar, más caro y complejo. 

Mientras seguían discutiendo sobre el estándar de OSI, TCP/IP ya se estaba usando...
```

## Nivel Físico


