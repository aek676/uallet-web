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
   Tras la incorporación, la nueva versión de la blockchain se distribuye a todos los nodos de la red, asegurando
   que todos posean la misma copia del libro mayor. Una vez que el bloque con su transacción ha sido confirmado,
   la transacción se considera definitiva.
