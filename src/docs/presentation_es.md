# UALlet

La nueva forma de hacer pagos de forma digital a través de blockchain
en todo el Campus de la UAL con 0% de comisión, 100% seguro y sin esperas.
Rápido, seguro y barato.

## 1. Introducción

En el campus de la Universidad de Almería existen varios locales (cafeterías,
kioskos, tiendas, papelerías, etc.) donde lo más común es realizar micropagos,
como un café (1.20$), fotocopias (0.10$), una barra pan (0.40$), etc.
La gran mayoría de estos pagos se realizan con tarjeta de crédito.

En este tipo de pagos, las comisiones de las tarjetas suelen
ser muy altas, llegando a ser incluso mayores que el importe de la compra.
Haciendo que los negocios tengan que asumir un gran coste o poner un mínimo
de compra, lo que puede ser un gran inconveniente para los clientes.

El sistema que proponemos es una aplicación donde los estudiantes podrán
pagar con un token propio de la universidad, que estará basado en la
tecnología blockchain, lo que permitirá realizar pagos de forma rápida, segura
y con comisiones muy bajas o incluso nulas. Además, este sistema también permitirá
a los estudiantes ganar recompensas al reducir los costos.

## 2. Blockchain

La tecnología blockchain es una base de datos digital (ledger) en la que se
registran cada transacción de forma pública y es mantenida por una red de ordenadores
distribuidos en todo el mundo. Por lo tanto es una red descentralizada.

Una blockchain es una cadena de bloques, cada bloque está vinculado cronológicamente
al bloque anterior, formando una cadena (chain). Un nuevo bloque contiene la transacción
más reciente y se añade a la cadena de bloques. Cada bloque tiene un hash único que lo
identifica, y el hash del bloque anterior, lo que garantiza la integridad de la cadena,
haciéndola inmutable.

Puntos claves:

- Las criptomonedas funcionan sobre blockchains y utilizan esta tecnología para procesar
  y asegurar las transacciones.

- Una blockchain ofrece un alto nivel de seguridad gracias a la criptografía, la
  descentralización, la transparencia y la inmutabilidad.

- Las transacciones se verifican mediante mecanismos de consenso, como Proof of Work (PoW)
  o Proof of Stake (PoS).

## 3. ¿Cómo funciona la blockchain?

Este es el proceso paso a paso:

1. Creación de una transacción

   Supongamos que quieres enviar bitcoins a otra persona. Crea la transacción desde su wallet,
   enviando bitcoins a la dirección del destinatario. La transacción incluye los siguientes datos:
   - Dirección pública del remitente y del destinatario.
   - Importe a transferir.
   - Información adicional.

2. Transmisión a la red

   Una vez creada se propaga en toda la red P2P de nodos, donde cada nodo recibe la misma información.

3. Verificación de la transacción

   Luego, la transacción es verificada por la red, que comprueba su validez. El método de verificación
   depende del mecanismo de consenso utilizado por la blockchain. Los más conocidos son:
   - Proof of Work: En el PoW, se utiliza potencia computacional para resolver complejos acertijos criptográficos.
     El ejemplo más conocido es la blockchain de Bitcoin.
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

## 4. Escalabilidad y costos

La escalabilidad se refiere a la velocidad con la que las blockchains pueden procesar
un gran número de transacciones. Cuanto más ocupado está el sistema, mayor es la
presión. Esto ha llevado a blockchains como Bitcoin y Ethereum a recibir muchas
críticas. Ambas blockchains funcionan haciendo que cada transacción sea validada
por toda la red. Esto limita el número de transacciones que pueden procesarse
por segundo.

[Escalabilidad de Bitcoin](https://chainspect.app/chain/bitcoin)

[Escalabilidad de Ethereum](https://chainspect.app/chain/ethereum)

¿Cómo Bitcoin fue desarrollado para ser un sustituto del sistema monetario cuando solo puede procesar aproximadamente 7
transacciones por segundo, mientras que sistemas como Visa pueden manejar miles por segundo?

Para abordar estos problemas se han desarrollado diferentes soluciones, tales como aplicar mejoras externas a Bitcoin y Ethereum,
haciéndolas más escalables, así como nuevas blockchains que son escalables por naturaleza:

- Soluciones de capa 2: Las soluciones de capa 2 permiten ejecutar transacciones
  fuera de la cadena principal y validarlas en bloque.
- Nuevos mecanismos de consenso: Como Proof of History de Solana y algoritmos innovadores
  de Proof-of-Stake.

## 5. Tipos de mecanismos de consenso

Para saber los diferentes tipos de mecanismos de consenso, es importante conocer
el funcionamiento de cada uno, para saber las ventajas y desventajas de cada uno,
y así poder elegir el más adecuado para cada caso de uso.

### 5.1. Proof of Work (PoW)

Proof of Work (PoW) es el mecanismo de consenso original de las blockchains,
utilizado por Bitcoin. Funciona mediante mineros que utilizan potencia
computacional para resolver complejos acertijos criptográficos. El primero
en encontrar la solución propone el nuevo bloque.

El proceso es el siguiente:

1. Las transacciones se agrupan en un bloque candidato.
2. Los mineros compiten para resolver un acertijo criptográfico (hash).
3. Cada intento requiere un nonce diferente hasta encontrar un hash válido.
4. El minero que encuentra la solución propaga el bloque a la red.
5. Otros nodos verifican la solución y si es válida, se añade a la cadena.

| Ventajas          | Desventajas             |
| ----------------- | ----------------------- |
| Seguridad         | Alto consumo energético |
| Descentralización | Menor escalabilidad     |
| Probado           | Costos de minería       |

### 5.2. Proof of Stake

Proof of Stake funciona mediante nodos y validadores. Un validador
es un nodo que participa activamente en la validación de transacciones
y la propuesta de nuevos bloques. Los validadores se seleccionan de forma
aleatoria en función de la cantidad de tokens que tienen en staking:
cuantos más tokens aportas, mayor probabilidad tienes a ser seleccionado
porque eres el que está jugándosela más, por tanto eres más confiable.
En principio, para participar en el staking algunas blockchains exigen
un mínimo y otras no.

El proceso es el siguiente: un validador es elegido de forma aleatoria
para añadir un bloque. Antes de hacerlo debe validar y procesar todas
las transacciones. Después de ello, tiene que llegar al consenso
validando con otros nodos, donde ellos revisan de forma independiente
el bloque y repiten la prueba criptográfica. Si todo es válido,
emiten una atestación y cuando llega al 51% se añade a la cadena.

| Ventajas              | Desventajas                                  |
| --------------------- | -------------------------------------------- |
| Eficiencia energética | Centralización                               |
| Escalabilidad         | Periodos de bloqueo de las monedas stakeadas |
| Accesibilidad         |                                              |

### 5.3. Proof of History

Proof of History es una tecnología desarrollada para resolver uno
de los problemas más difíciles de las blockchains: establecer un
orden temporal fiable y descentralizado de los eventos. PoH es una
adición al PoS ya existente. Fue desarrollado por Solana para
abordar el problema que requieren mucha comunicación para determinar
que transacción ocurrió primero. PoH registra el orden cronológico
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

3. Construir bloques
   - El validador al que le toca utiliza la secuencia de PoH para
     ordenar las transacciones.
   - Como el orden ya viene fijado, los validadores ya no necesitan
     ponerse de acuerdo sobre el orden, lo que ahorra tiempo.

4. Procesar el consenso
   - Otros validadores revisan la secuencia de PoH y las transacciones.
   - Solana utiliza Tower BFT
   - Tras obtener suficientes votos, el bloque se vuelve definitivo

### 5.4. Comparativa de mecanismos de consenso

Ya hemos descrito los tres mecanismos de consenso más populares, ahora vamos a compararlos:
Para ello nos vamos a meter en la siguiente página donde podremos comparar los diferentes
mecanismos de consenso.

[Blockchain Scalabity](https://chainspect.app/dashboard)

Donde podremos ver que la opción más adecuada para nuestro caso de uso es Solana.

## 6. Comparativa de precios

Vamos a hacer una comparativa de precios entre las diferentes
blockchains y los métodos de pago tradicionales, para ver la
diferencia de costes entre ellos.

### 6.1. On-chain

|          | Coste                   | Fuente                                      |
| -------- | ----------------------- | ------------------------------------------- |
| Bitcoin  | $0.3664                 | [Fee](https://mempool.space/)               |
| Ethereum | $0.073                  | [Fee](https://etherscan.io/gastracker)      |
| Solana   | 0.000005 SOL = $0.00036 | [Fee](https://solana.com/es/docs/core/fees) |

### 6.2. Off-chain

|             | Coste              | Fuente                                                     |
| ----------- | ------------------ | ---------------------------------------------------------- |
| TPV Físico  | 0,20% + 12€/mes    | Sabadell                                                   |
| TPV Virtual | 0,40% + 9€/mes     | Sabadell                                                   |
| Pay by Bank | Muy bajos por PSD2 | [Tink](https://tink.com/es/productos/iniciacion-de-pagos/) |

## 7. Objetivos

El objetivo de este proyecto es el desarrollo de una aplicación móvil
que permita a los negocios no tener que asumir gastos por pagos TPV y
a los estudiantes poder realizar pagos de forma digital sin tener que
enfrentarse a las restricciones de los pagos tradicionales.

Fuck TPVs

### 7.1. Principales problemas

El principal problema que nos podemos encontrar es la adopción de la
aplicación, por tanto para ello se podrían ofrecer incentivos a los
estudiantes para que la usen, como por ejemplo

- Cada vez que un estudiante realice un pago con la aplicación,
  recibirá una recompensa en forma de NFT que podrán canjear por descuentos
  en los locales del campus o por otros beneficios.

Otro problema al que nos podemos enfrentar es la forma de pasar dinero
off-chain a on-chain, para ello se han pensado diferentes soluciones, como por ejemplo:

- Una pasarela de pago con Redsys o Stripe, que permitan a los estudiantes comprar
  tokens con dinero fiat. Pero esta no es una opción muy viable, ya que una
  pasarela de pago nos cobra más comisión que un TPV físico.

- Otra opción que se ha barajado es utilizar transferencias bancarias mediante SEPA,
  donde las comisiones suelen ser muy bajas o casi nulas. Esta es la opción más
  viable.

### 7.2. Formas de pasar dinero on-chain a off-chain

Se hizo una investigación para saber cuáles son las formas más eficientes
y baratas para poder pasar dinero líquido a dinero digital o cripto.

La primera opción fue usar una pasarela de pago, como por ejemplo Redsys o Stripe,
pero esta opción no es viable, ya que al utilizar una pasarela de pago se nos cobra
más comisión que pagar con un TPV físico. Además de pagos con Bizum, pero
es lo mismo.

También nos encontramos con la opción de [Stripe](https://stripe.com/en-es/use-cases/crypto)
que permite convertir dinero fiat a una stable coin, pero
esta opción también tiene comisión.

La opción más viable que encontramos fue la que utilizan
proyectos como [Monerium](https://monerium.com/) o [Circle](https://www.circle.com/es-la/circle-mint)
que permiten convertir dinero fiat a dinero digital (Mint) mediante
transferencias bancarias, donde las comisiones suelen ser muy bajas o casi nulas.

Pero esta opción al usuario final no le puede ser la más cómoda, ya que tendría
que entrar a su aplicación del banco y poner tanto el IBAN de destino como indicar
su billetera y datos relevantes para que se efectúe el Mint.

Por tanto, podemos usar la opción de [Tink](https://tink.com/es/productos/iniciacion-de-pagos/),
la cual usa Openbanking y hace los pagos automáticamente,
mediante transferencias bancarias. Además de que las comisiones
son muy bajas.

### 7.3. Token

Para el token del campus se ha pensado en hacerlo stable coin,
para evitar la volatilidad de las criptomonedas, y que su valor
sea siempre el mismo, por ejemplo 1 token = 1 euro. Esto se conseguiría
montando una tesorería con dinero real en la cual mediante un contrato
inteligente que haga lo siguiente:

- Cuando el estudiante transfiera dinero a la tesorería se acuñe (Mint)
  tokens a la wallet del estudiante.
- Cuando quiera intercambiar tokens por dinero se queman (Burn) los tokens
  y se transfiere el dinero de la tesorería.

### 7.4. Regulación (Ley MiCA)

La [Ley MiCA](https://eur-lex.europa.eu/ES/legal-content/summary/european-crypto-assets-regulation-mica.html) (Markets in Crypto-Assets)
es una regulación europea que entró en vigor en 2023
y se aplica completamente desde diciembre 2024. Esta regulación
establece requisitos para los emisores de crypto-activos y los proveedores de servicios.

Sin embargo, al tratarse de un token de **uso cerrado** (solo válido dentro del
campus), no aplicaría esta regulación, ya que:

- El token no puede intercambiarse fuera del campus
- No es un instrumento financiero tradicional
- No se utiliza para inversiones o pagos externos

Sería como usar una tarjeta de Zara. Por tanto, el proyecto podría
operar bajo el marco de la normativa sin necesidad de licencias
especiales de MiCA.

## 8. Funcionamiento de la aplicación

Sería una aplicación enfocada a móviles, donde los estudiantes
podrían recargar su cuenta y hacer pagos o cobros.

1. El estudiante recarga su cuenta mediante Pay by Bank.
2. El estudiante recibe sus tokens en su cuenta/wallet.
3. El estudiante puede hacer pagos con la cuenta, mediante un código QR
   utilizando [Solana Pay](https://www.youtube.com/watch?v=5uABl49jknk)
4. Si un estudiante quiere pasar tokens a dinero no podrá. La única forma es
   hacer un intercambio con otro estudiante. Esta opción solo estará habilitada
   para los comercios.

## 9. Ventajas

La principal ventaja, aparte de ofrecer pagos con 0 comisiones, es que este
sistema se puede implementar a pagos de espacios deportivos, excursiones, etc.

Además, se podrían implementar otras funcionalidades, como por ejemplo:

- Becas Comedor: El programa actual ingresa euros a la cuenta del alumno.
  Nada impide que el alumno se gaste este dinero en ropa o salir de fiesta.
- Identidad Digital: Cada alumno podría tener su identidad digital en su
  wallet, lo que permitiría acceder a servicios de la universidad de forma
  más rápida y segura.
- Gobernanza y Votaciones: Si cada alumno tiene su wallet, se puede crear
  un sistema de votos anónimo, infalsificable, transparente y auditable en
  tiempo real.

Y la más importante, ser la primera universidad de España en implementar
un sistema de pagos basado en blockchain.

## Fuentes

- [¿Qué es una blockchain?](https://finst.com/es/learn/articles/what-is-blockchain)
- [Proof of Work](https://finst.com/es/learn/articles/what-is-proof-of-work)
- [Proof of Stake](https://finst.com/es/learn/articles/what-is-proof-of-stake)
- [Proof of History](https://finst.com/es/learn/articles/what-is-proof-of-history)
