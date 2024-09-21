# Proyecto3-Riesgo Relativo
## Índice

- [1. Contexto](#contexto)
- [2. Objetivo](#objetivo)
- [3. Metodología](#metodología)
  [3.1 Procesamiento y preparación de datos](#procesamiento-y-preparación-de-datos)
- [3.2 Análisis exploratorio](#análisis-exploratorio)
- [3.3 Análisis de riesgo relativo](#análisis-de-riesgo-relativo)
- [4. Visualización de resultados](#visualización-de-resultados)
- [5. Conclusiones](#conclusiones)
- [6. Recomendaciones](#recomendaciones)
- [6. Enlaces de recursos](#enlaces-de-recursos)

## 1. Contexto: 
Una discográfica se enfrenta al emocionante desafío de lanzar un nuevo artista en el escenario musical global.
## 2. Objetivo:
En este proyecto se analizó el riesgo relativo en una base de datos de clientes de un banco, para la segmentación e identificación de psoibles buenos y malos pagadores. El objetivo principal es mejorar la eficiencia y la precisión en la evaluación del riesgo crediticio, permitiendo al banco tomar decisiones informadas sobre la concesión de crédito y reducir el riesgo de préstamos no reembolsables.
## 3. Metodología:
  ## 3.1 Procesamiento y preparación de datos:
* 1. Herramientas:
Hojas de cálculo de Google
Gran consulta
Estudio Looker
ChatGPT
Lienzo
Presentaciones de Google
Telar
* 2. Idiomas:
SQL y BigQuery
* 3. Descripción de las fuentes de datos:
Este conjunto de tablas contiene información sobre préstamos concedidos a un grupo de clientes del banco, los cuales se dividen en:

* user_ info	

user_ id	Número de identificación del cliente (único para cada cliente)
age	Edad del cliente
sex	Sexo del cliente
last_ month_ salary	Último salario mensual que el cliente reportó al banco
number_dependents	Número de dependientes

* loans_ outstanding	

loan_ id	Número de identificación del préstamo (único para cada préstamo)
user_ id	Número de identificación del cliente
loan_ type	Tipo de préstamo (real estate = inmobiliario, others = otro)

* loans_ detail

user_ id	Número de identificación del cliente

more_ 90_ days_ overdue	Número de veces que el cliente estuvo más de 90 días vencido

using_ lines_ not_ secured_ personal_ assets	Cuánto está utilizando el cliente en relación con su límite de crédito, en líneas que no están garantizadas con bienes personales, como inmuebles y automóviles

number_ times_ delayed_ payment_ loan_ 30_ 59_ days	Número de veces que el cliente se retrasó en el pago de un préstamo (entre 30 y 59 días)

debt_ ratio	Relación entre las deudas y el patrimonio del prestatario. Ratio de deuda = Deudas / Patrimonio

number_ times_ delayed_ payment_ loan_ 60_ 89_ days	Número de veces que el cliente retrasó el pago de un préstamo (entre 60 y 89 días)

* default

user_ id	Número de identificación del cliente
default_ flag	Clasificación de los clientes morosos (1 para clientes que pagan mal, 0 para clientes que pagan bien)

## 4. Visualización y análisis de datos:
