# Similitud-de-documentos

##### Este código tiene como objetivo comparar documentos a través de su representación vectorial en Python. Para ello, se utilizan las bibliotecas scikit-learn y spaCy. La representación vectorial se realiza mediante tres técnicas diferentes: binarización, frecuencia y TF-IDF.
- El corpus de noticias se lee desde un archivo llamado corpus_noticias_procesado.txt. Además, se define una lista de stop words que se utilizará para el procesamiento de los documentos.
- El primer paso es la representación vectorial binarizada de los documentos. Para ello, se utiliza la clase CountVectorizer de scikit-learn con el parámetro binary=True. El resultado de esta representación vectorial se almacena en la variable X_binario.
- El segundo paso es la representación vectorial por frecuencia de los documentos. Para ello, se utiliza la misma clase CountVectorizer de scikit-learn sin el parámetro binary. El resultado de esta representación vectorial se almacena en la variable X_frecuencia.
- El tercer paso es la representación vectorial TF-IDF de los documentos. Para ello, se utiliza la clase TfidfVectorizer de scikit-learn. El resultado de esta representación vectorial se almacena en la variable X_tfidf.
- Finalmente, se lee la noticia que se desea comparar desde un archivo llamado noticia.txt. Se realiza su procesamiento y se almacena en la variable df_noticia. Luego, se calcula la similitud entre la noticia y cada uno de los documentos del corpus mediante la función cosine_similarity.
- Es importante destacar que este código puede ser utilizado para la comparación de cualquier tipo de documentos, no sólo noticias, simplemente cambiando el corpus y la noticia de ejemplo por otros documentos de interés. Además, se pueden ajustar los parámetros de las clases de scikit-learn utilizadas para obtener diferentes representaciones vectoriales y mejorar los resultados de la comparación.
