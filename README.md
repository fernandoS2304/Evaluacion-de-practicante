# Evaluacion-de-practicante
Desarrollo del test de evaluacion para el puesto de practicante de informática bolsa de trabajo PUCP
Primero cada uno de los campos los convertimos en arreglos para tener un mejor manejo de estos
Luego verificamos que los datos esten bien colocados y que no se hayan alterado
Se utiliza el tokenize en la descripción para limpiar la data y asi poder realizar mejor el TF IDF
Se realiza el codigo del TF IDF con lo cual obtenemos el vector X que se usara para el clasificador bayesiano
Ya que para usar el clasificador se necesitan números, primero se ve cuales son las posiones que exiten y luego se le otorga un número a cada una
Se realiza el cambio en la base de datos y creamos el vector Y que es del "Position Level" para poder usar nuestro clasificador
Se crea el data train con el 25% de la base de datos total y también se crea el data test
Al usar el clasificador bayesiano (Bernoulli) el score es demasiado bajo, por lo que decidí probar otros clasificadores, siendo el SGD el que tuvo el mayor score
Esto se puede deber a data desvalanceada, lo que se puede arreglar usando metodos undersampling o oversampling para valancear la data y obtener mejores resultados
