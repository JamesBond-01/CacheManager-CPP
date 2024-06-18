# Cache Manager

Se implementará un cache manager, que se salvará un
pair compuesto por clave y valor, ambos en RAM y en disco (files).
Dada una clave, el cache manager accede al valor. Si el valor existe en
la memoria es retornado. En caso que no exista en memoria, entonces
el cache deberá buscar la clave en el archivo y retornar el pair si es
encontrado.

El caché también debe implementar un tamaño límite de capacidad, lo
que significa una restricción sobre cuántos elementos pueden existir a la
vez en la memoria. Una vez que se ha alcanzado el límite, el menos utilizado recientemente (LRU) debe eliminarse de la memoria para ingresar
al nuevo.

En el momento de la inserción, todo nuevo par < key; valor > debe
guardarse tanto en la memoria como en el archivo.
