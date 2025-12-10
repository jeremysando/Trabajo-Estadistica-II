# Estadística
Este repositorio contiene la base de datos limpia utilizada para el análisis de la confianza en la Policía Nacional del Perú, elaborada a partir de la encuesta LAPOP 2023. El proceso incluye selección, renombrado y recodificación de variables relevantes para el procesamiento del futuro modelo.

En el proceso de limpieza y preparación de datos, varias variables del cuestionario LAPOP 2023 (Perú) fueron recodificadas a formato binario (0 y 1) con el fin de facilitar la interpretación del futuro modelo. En primera instancia, las transformaciones realizadas fueron las siguientes:


| Variable original | Nueva variable            | Descripción                                                               | Recodificación                                                                    |
| ----------------- | ------------------------- | ------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| **B18**           | `confianza_policia`       | Nivel de confianza en la Policía Nacional del Perú.                       | 1 = Confía (valores 5, 6, 7) / 0 = No confía (1–4)                                |
| **VIC1EXT**       | `victimizacion`           | Indica si la persona fue víctima de algún delito en los últimos 12 meses. | 1 = Sí / 0 = No                                                                   |
| **AOJ11**         | `inseguridad`             | Percepción de inseguridad en el barrio o comunidad.                       | 1 = Percibe inseguridad (valores 3 y 4) / 0 = No percibe (1 y 2)                  |
| **PN4**           | `satisfaccion_democracia` | Grado de satisfacción con la democracia en el país.                       | 1 = Satisfecho o muy satisfecho (1–2) / 0 = Insatisfecho o muy insatisfecho (3–4) |
| **SEXIN**         | `sexo`                    | Sexo de la persona encuestada.                                            | 1 = Hombre / 0 = Mujer (excluye “No se identifica”)                               |


A continuación, el diccionario de datos: 

| Variable                 | Descripción                                           | Tipo        | Codificación |
|---------------------------|-------------------------------------------------------|-------------|---------------|
| Confianza_policia         | Nivel de confianza en la Policía Nacional del Perú   | Binaria     | 1 = Confía / 0 = No confía |
| Victimizacion             | Si fue víctima de delito en los últimos 12 meses     | Binaria     | 1 = Sí / 0 = No |
| Inseguridad               | Percepción de inseguridad en su barrio               | Binaria     | 1 = Inseguro / 0 = Seguro |
| Satisfaccion_democracia   | Nivel de satisfacción con el funcionamiento democrático | Binaria  | 1 = Satisfecho / 0 = Insatisfecho |
| Sexo                      | Sexo del encuestado                                 | Categórica  | Hombre / Mujer |
| Edad                      | Edad del encuestado                                 | Numérica    | Continua |
| Nivel_educativo           | Nivel educativo alcanzado                           | Categórica  | Baja / Media / Alta |


De igual manera, al ser mi html muy pesado y no poder abrirse, lo he subido a RPubs con el objetivo de que se visualice:
https://rpubs.com/JeremySando/1379176
