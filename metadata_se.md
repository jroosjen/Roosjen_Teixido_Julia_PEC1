# Metadatos del objeto de clase `SummarizedExperiment`

Este archivo contiene toda la información relevante sobre los metadatos de objeto de clase `SummarizedExperiment` que se ha utilizado en esta PAC

## 1. Metadatos generales del estudio

La siguiente información se ha encontrafo con la función `metadata(se)`:

$data_source
[1] "Metabolomics Workbench"

$study_id
[1] "ST000002"

$analysis_id
[1] "AN000002"

$analysis_summary
[1] "GCMS positive ion mode"

$units
[1] "Peak height"

$name
[1] "ST000002:AN000002"

$description
[1] "Intestinal Samples II pre/post transplantation"

$subject_type
[1] NA

Esta función da como resultado una lista de toda la información adicional del ensayo. Como de donde provienen los datos, el identificador del estudio, el identificador del analisis realizado (GCMS positive ion mode), las unidades con las que se miden los datos, o una descripción del estudio.


## 2. Metadatos de las columnas (las muestras)

Para obtener la metadata de las columnas se utiliza la función `colData(se)`:

- local_sample_id
- study_id
- sample_source
- mb_sample_id
- raw_data
- Transplantation

A partir de esta metadata se puede encontrar información adicional sobre las muestras tomadas. Podemos identificar el local_sample_id que seria la etiqueta de cada muestra sin el _A o _B que se le ha añadido. También encontramos el id del estudio junto a la procedencia de la muestra (intestino). Además podemos identificar el id del analisis que se ha realizado en cada muestra, junto a la información sobre si la muestra se tomó antes o despues del trasplante.


## 3. Metadatos de las filas (metabolitos)

Para obtener la metadata de las filas se utiliza la unción `rowData(se)`:

- metabolite_name
- metabolite_id
- refmet_name

A partir de la metadata de las filas podemos encontrar información adicional sobre los metabolitos. Con la metadata encontramos el nombre de cada uno de los metabolitos correspondiente al identificador de los datos. También, encontramos el nombre de referencia de los metabolitos.
