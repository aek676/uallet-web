# UALlet

La nueva forma de hacer pagos de forma digital através de blockchain
en todo el Campus de la UAL con 0% comision, 100% de seguro y sin esperas.
Rápido, seguro y barato.

## 1. Introducción

Vamos a explicar como vamos a hacer esto, además de explicar toda la evolución
de la blockchain y como se ha llegado a este punto de pagar de forma insntantenea
y casi sin comisiones.

## 2. Blockchain

La tecnología blockchain es una base de datos digital (leadger) en la que se
registran cada transacción de forma pública y es mantenida por una red de ordenadores
distribuidos en todo el mundo. Por lo tanto es una red descentralizada.

Una blockchain es una cadena de bloques, cada bloque esta vinculado cronológicamente
al bloque anterior, formando una cadena (chain). Un nuevo bloque contiene la transacción
más reciente y se añade a la cadena de bloques. Cada bloque tiene un hash único que lo
identifica, y el hash del bloque anterior, lo que garantiza la integridad de la cadena,
haciendola inmutable.

Puntos claves:

- Las criptomonedas funcionan sobre blockchains y utilizan esta tecnlogía para procesar
  y asegurar las transacciones.

- Una blockchain es ofrece un alto nivel de seguridad gracias a la criptografía, la
  descentralización, la transparencia y la inmutabilidad.

- Las transacciones se verifican mediante mecanismos de conseso, como Proof of Work (PoW)
  o Proof of Stake (PoS).

## 3. ¿Comó funciona la blockchain?

Este es el proceso paso a paso:

1. Creación de una transacción

   Supongamos que quieres enviar bitcoins a otra persona. Crea la transacción desde su wallet,
   enviando bitcoins a la dirección del destinatario. La transacción incluye los siguientes datos:
   - Dirección pública del remitente y del destinatario.
   - Importe a transferir.
   - Información adicional.

2. Transmición a la red

   Una vez creada se propaga en toda la red P2P de nodos. Donde cada nodo recibe la misma información.

3. Verificación de la transacción

   Luego, transacción es verificada por la red, que comprueba su validez. El método de verificación
   depende del mecanismo de consenso utilizado por la blockchain. Lo mas conocidos son:
   - Proof of Work: En el PoW, se utiliza potencia computacional para resolver complejos acertijos criptográficos.
     El ejemplo mas conocido es la blockchain de Bitcoin.
   - Proof of Stake: En el PoS, los participantes "apuestan" sus monedas para validar transacciones. Es más eficiente
     energéticamente. Un ejemplo de blockchain que utiliza PoS es Ethereum 2.0.

4. Agrupación en un bloque
   Una vez validadas las transacciones se agrupan en un bloque. Este bloque será propuesto por un nodo para su
   incorporación a la cadena.

5. Incorporación del bloque a la blockchain
   El nuevo bloque se añade a la cadena de bloques. Contiene un enlace al bloque anterior, manteniendo así la
   continuidad de la cadena. Una vez añadido, los datos del bloque no pueden ser modificados.

6. Confirmación del bloque
   Tras la incorporación, la nueva versión de la blockchain se distribuye a todos los nodos de la red, asegurando que todos posean la misma copia del libro mayor. Una vez que el bloque con su transacción ha sido confirmado, la transacción se considera definitiva.

## 4. Escabilidad y costos

La escabilidad se refiere a la velocidad con la que las blockchains pueden procesar
un gran número de transacciones. Cuanto más ocupado está el sistema, mayor es la
presión. Esto ha llevado a blockchains como Bitcoint y Ethereum a recibir muchas
críticas. Ambas blockchains funcionan haciendo que cada transacción sea validada
por toda la red. Esto limita el número de transacciones que pueden procesarse
por segundo.

[Escalabilidad de Bitcoin](https://chainspect.app/chain/bitcoin)
[Escalabidad de Ethereum](https://chainspect.app/chain/ethereum)

¿Comó Bitcoin fue desarrollado para ser un sustituto del sistema monetario cuando solo puede procesar aproximadamente 7
transacciones por segundo, minetras que sistemas como Visa pueden manejar miles por segundo?

Para abordar estos problemas se han desarrollado diferentes soluciones, tales como aplicar submejoras a Bitcoin y Ethereum
más escalables, así como nuevas blockchains que son escalables por naturaleza:

- Soluciones de capa 2: Las soluciones de capa 2 permiten ejecutar transacciones
  fuera de la cadena princpipal y validarlas en bloque.
- Nuevos mecanismos de consenso: Como Proof of History de Solana y algoritmos innovadores
  de Proof-of-Stake.

## 5. Tipos de mecanismos de consenso

Para saber los diferentes tipos de mecanismos de consenso, es importante conocer
el funcionamiento de cada uno, para saber la ventajas y desventajas de cada uno,
y así poder elegir el más adecuado para cada caso de uso.

### 5.1. Poof of Work (PoW)

...

### 5.2. Proof of Stake

Proof of Stake funciona mediante nodos y validadores. Un validador
es un nodo que participa activamente en la validación de transacciones
y la propuesta de nuevos bloques. Los validadores se seleccionan de forma
aleatorio en funcion de la cantidad de tokens que tienen en staking:
cuantós más tokens aportas, mayor probabilidad tienes a ser seleccionado
porque eres el que esta jugandosela más, por tanto eres más confiable.
En principio, para participar en el staking algunas blockchains exigen
mínimo y otras no.

El proceso es el siguiente: un validador es elegido de forma aleatoria
para añadir un bloque. Antes de hacerlo debe validar y procesar todas
las transacciones. Después de ello, tiene que llegar al conseso
validando con otros nodos, donde ellos revisan de forma independiente
el bloque y repiten la prueba criptográfica. Si todo es válido,
emiten una atestación y cuando llego al 51% se añade a la cadena.

| Ventajas              | Desventajas                                   |
| --------------------- | --------------------------------------------- |
| Eficiencia energética | Centralización                                |
| Escalabilidad         | Periodos de bloqueo de las monendas stakeadas |
| Accesibilidad         |                                               |

### 5.3. Proof of History

Proof of History es una tecnología desarrollada para resolver uno
de los problemas más difíciles de las blockchains: establecer un
orden temporal fiable y descentralizado de los eventos. PoH es una
adicción al PoS ya existente. Fue desarrollado por Solana para
abordar el problema que requieren mucha comunicación para determinar
que transacción ocurrión primero. PoH registra el orden cronológico
antes de que se alcance el consenso, abordando así este problema.

El proceso es el siguiente:

1. Generar la cadena de hashes
   - Se aplica repetidamente una función de hash criptográfico (SHA-256)
     donde la salida del paso anterior se convierte en la entrada del siguiente.
   - Cada hash es único y solo puede calcularse recorriendo todos los hashes
     anteriores, lo que crea una secuencia verificable.
   - Esto genera un reloj criptográfico: una serie de sellos de tiempo que
     cualquiera pueda verificar.

2. Insertar eventos y transacciones
   - Las nuevas transacciones se insertan en la cadena de hashes.
   - Esto permite determinar el orden cronológico de cuando ocurrió
     cada evento.

3. Contruir bloques
   - El validador al que le toca utiliza la secuencia de PoH para
     ordenar las transacciones.
   - Como el orden ya viene fijado, los validadores ya no necesitan
     ponerse de acuerdo sobre el orden, lo que ahorra tiempo.

4. Procesar el consenso
   - Otros validadores revisan la secuencia de PoH y las transacciones.
   - Solana utiliza Tower BFT
   - Tras obtener suficientes votos, el bloque se vuelve definitivo

## Fuentes

- [¿Qué es una blockchain?](https://finst.com/es/learn/articles/what-is-blockchain)
- [Proof of Work](https://finst.com/es/learn/articles/what-is-proof-of-work)
- [Proof of Stake](https://finst.com/es/learn/articles/what-is-proof-of-stake)
- [Proof of History](https://finst.com/es/learn/articles/what-is-proof-of-history)
