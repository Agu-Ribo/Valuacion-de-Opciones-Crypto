# Valuacion-de-Opciones-Crypto
El objetivo de este trabajo es investigar las particularidades de los contratos de opciones de criptomonedas, asi como también encontrarles un precio mediante la aplicación de modelos matemáticos utilizados en las finanzas tradicionales: el modelo de Black-Scholes &amp; Merton, Modelo de Arbol Binomial y Monte Carlo. Para hallar dicho precio, se utiliza la librería de Python denominada QuantLib.

El reciente aumento de la capitalización de mercado de las criptomonedas -market capitalization-  (2.3 Trillons U$S)  y su creciente popularidad han diseñado y perfeccionado una serie de instrumentos  derivados financieros, tales como Opciones de Bitcoin, Futuros de Bitcoin y Perpetuos. 
La aparición de los contratos de futuros y opciones de Bitcoin han recibido considerable atención en este último tiempo. Estos contratos han sido utilizados por inversores particulares como instrumentos de cobertura y de especulación. 
Los contratos de opciones de bitcoin se encuentran en una incipiente etapa de desarrollo temprana y son operados solamente en algunos exchanges (tales como Binance , OKEx  o Deribit , siendo este último el que más productos de derivados ofrece y el de mayor capitalización de los mismos).
La valuación de opciones juega un rol fundamental en el manejo de portfolios. Provee un pronóstico base que asiste a la rigurosa toma de decisiones para el portfolio managment. Clave, cuando se tratan de mercados tan volátiles e inmaduros como el de bitcoin. El más popular y ampliamente aceptado, el modelo de fijación de precios de opciones de Black-Scholes (Black y Scholes 1973) para determinarle un precio justo a un contrato de opción es el mas estudiado. El estudio de las opciones no se limita a opciones de acciones y bonos; existe un cuerpo extraordinariamente ancho y profundo de la literatura que también examina opciones de divisas, opciones de commodities e incluso opciones de tasa de interés.

Conceptos

Criptomoneda: Es el nombre dado a un medio digital de pago basado en herramientas criptográficas, tal como cadenas de bloques –blockchains- y firmas digitales. Como medio de pago, pretende ser descentralizado, es decir independiente, distribuido y seguro. La crypto más conocida es Bitcoin.
Cadena de bloques: Es una base de datos distribuida y pública. Consiste en bloques de datos que están conectados entre sí en orden cronológico. Una analogía sencilla es una novela: el texto son los datos, la página es el bloque y el encuadernado es la blockchain.
Contrato Inteligente: Se le dice Contrato Inteligente (Smart Contract) al software o programa ubicado en la blockchain. Pensemoslo como un procedimiento programado. Si ciertas condiciones se cumplen, el procedimiento se lleva a cabo automáticamente.

Opciones Financieras: existen dos tipos básicos de opciones. Una opción de compra – call - le da al tenedor de la opción el derecho a comprar el activo subyacente a un precio (strike) y fecha (vencimiento) previamente determinados. Por el otro lado, una opción de venta – put – le da al tenedor de la opción el derecho a vender el activo subyacente a un precio y fecha previamente determinados. 
Las opciones pueden ser también del tipo Americanas o Europeas. Las primeras tienen la particularidad de que pueden ser ejercidas en cualquier momento hasta su expiración, en cambio las del tipo Europeo solo podrán serlo en el día de su vencimiento.
El precio que nosotros pagamos cuando compras una opción, ya sea de compra o de venta, se lo denomina “prima”

Factores que influyen en el precio de las Opciones
Para la determinación del precio de una opción, son varios los factores que influyen, como ser:
1)	El precio actual de la acción (S0)
2)	El precio del ejercicio (K)
3)	El tiempo al vencimiento (T)
4)	La volatilidad del precio de la acción (σ)
5)	La tasa de interés libre de riesgo (r)

Volatilidad: mide las fluctuaciones en el precio de un instrumento financiero en un período de tiempo predeterminado. Se calcula como la Desviación Estandar de los Rendimientos Logarítmicos utilizando los precios de cierre diarios.

Volatilidad Implícita (VI): representa las fluctuaciones esperadas en el precio de un instrumento financiero en un período predeterminado en el futuro. La VI es calculada en base al precio de las opciones de un instrumento subyacente. Dado que el precio de las opciones está directamente relacionado al nivel de la Volatilidad Implícita, éste es un indicador de expectativas que tiene el mercado acerca de la volatilidad del instrumento subyacente. 
