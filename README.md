# README Big Data Project
## Introducción
El siguiente código recoje tweets de cierto tema o hastag, y los compila en un DataFrame. Luego, los tweets son preprocesados y posteriormente se realiza el análisis de sentimiento. 
El objetivo es poder visualizar la opinión popular de una empresa, organización, o entidad — teniendo en cuenta las menciones en las redes sociales.

## Pre-requisitos:
1. - Aplicaciones de procesado de planillas (tales como Microsoft Office o G Suite).
2. - IDE (o similar) compatible con las librerías utilizadas.
3. - Una Application Key de la API de Twitter (necesario para poder acceder a los tweets).

## Instalación:
Se puede ejecutarse desde Google Collab, o desde cualquier IDE compatible.

## Environment:
Language : Python

Libraries : 
- tweepy
- os
- pandas
- google collab (files)
- io
- matplotlib (pyplot)
- seaborn
- itertools
- collections
- nltk
- re
- networkx
- textblob
- warnings
- numpy

## Algoritmo de Análisis de Sentimiento utilizados
El algoritmo utilizado fué el de polaridad. Elegimos este análisis debido a que nos dá a conocer qué tipo de percepción (positiva o negativa), y por ende, como se sienten acerca de los distintos temas buscados — mediante el  uso de distintos hashtags. Creemos que el análisis de polaridad es muy útil a la hora de calcular la aprobación o rechazo de un nuevo producto, un nuevo servicio, o de una compañía en general. Utilizando distintos parámetros de tiempo, podemos ver un panorama histórico de los sentimientos de los clientes.

## Preprocesamiento de datos
- 1. Remoción de menciones @: Todos los '@unnombre' no sirven de nada ya que no transmiten ningún significado.
- 2. Remoción de links: Los enlaces en el texto no sirven de nada porque tampoco transmiten ninguna información útil.
- 3. Remoción filas redundantes: Las filas redundantes o duplicadas son innecesarias para nuestro análisis.
- 4. Remoción puntuaciones, números, y carácteres especiales: Este tipo de carácteres no son necesarios para el análisis.
- 5. Remoción de stopwords: Las palabras de parada son las que se utilizan sólo para la formación correcta de la frase. No tienen ningún significado de información completa. Por lo tanto, es necesario eliminarlas para que nuestro registro de texto sea más limpio.
- 6. Tokenización y Lematización: - Tokenización: conversión de los fragmentos de texto en palabras individuales. - Lematización: proceso en el que tomamos tokens individuales de una frase y tratamos de reducirlos a su forma básica. - Ambos procesos mejoran los resultados del procesamiento de lenguaje natural, debido a que facilitan la interpretación del tweet.

## Resultado:
Una vez ejecutado el script, el output deberian ser dos archivo csv: uno con los tweets no procesados y sus atributos, y otro con los tweets procesados y con su índice de polaridad.

## Autores:
- Abel Ezequiel Valotta Moulard | UPA - TIE| Cohorte 2019 
- Pablo Daniel Pedrozo Ramírez | UPA - TIE| Cohorte 2019 

## Fecha:
Junio, 2021

### *End*
