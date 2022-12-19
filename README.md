# Flask-SQL
## Paso 1
### Creamos el entorno virtual correspondiente
Creamos el entorno con el siguiente comando
![image](https://user-images.githubusercontent.com/114931679/208457750-5a244450-f3de-4a45-adbc-7923e9132e90.png)

Establecemos la directiva de ejecución en un ámbito determinado, y lo activamos para instalar las herramientas necesarias.
![image](https://user-images.githubusercontent.com/114931679/208457570-34337169-7807-4b9f-92c2-d9e6872fd1bc.png)

Creamos el archivo .py 
Instalamos flask, flask_alchemy con el comando _**import**_
![image](https://user-images.githubusercontent.com/114931679/208458847-c959a7e5-c464-4dce-9aaf-b3dad7c5b2c1.png)

Mediante _**config**_ configuramos nuestra base de datos
![image](https://user-images.githubusercontent.com/114931679/208459804-0dcbd9ba-86b0-474d-a413-464abfb754ff.png)

### Ahora crearemos las tablas de la base de datos, es decir los modelos
![image](https://user-images.githubusercontent.com/114931679/208463099-e03575b7-44f9-4e71-9bab-af5942734927.png)
![image](https://user-images.githubusercontent.com/114931679/208463166-27a29413-2076-4c98-868f-54b41b02350e.png)
![image](https://user-images.githubusercontent.com/114931679/208463211-bf7dc3e5-50c3-4acf-95fd-b3cfcf9b7449.png)


Podemos observar que la primary_key es la columna id en las 3 tablas.
Las columnas que no pueden recibir un valor nulo contienen nullable con valor False.
Las columnas que son únicas contienen la palabra unique con valor True.

### Siguiente paso será establecer la relación entre las tablas
![image](https://user-images.githubusercontent.com/114931679/208462862-0303e666-6d76-4e1c-ab02-3bbf0e956cb3.png)
![image](https://user-images.githubusercontent.com/114931679/208462948-b87c0c33-21ad-4d73-90df-02b7d4020fc0.png)
![image](https://user-images.githubusercontent.com/114931679/208463013-17175ad0-0919-4ea9-b2c0-77d78eaa5052.png)

### instalamos sqlite y extraemos los ficheros
![image](https://user-images.githubusercontent.com/114931679/208466426-2e8345b2-29fe-49e1-b113-0c68f0548977.png)

Tenemos que crear la carpeta sqlite 3 en el disco duro local C: y copiar los archivos extraidos
![image](https://user-images.githubusercontent.com/114931679/208467666-60e97ea2-d81d-49b5-b2e2-bcdd2514ddd4.png)
Ahora podremos abrir sqlite desde cualquier terminal.

Accedemos a la consola Flask con el comando _**flask shell**_ y ejecutamos las instancias
![image](https://user-images.githubusercontent.com/114931679/208471043-9f5d76a9-d041-428f-9c6d-54e6c8cba082.png)

y ahora accedemos a las tablas
![image](https://user-images.githubusercontent.com/114931679/208471604-46ff9977-5170-49ee-bdbb-629edc7af49f.png)
![image](https://user-images.githubusercontent.com/114931679/208471703-66188a63-244a-4caf-b311-846c39b2e7d1.png)

### Desde el tutorial existe una funcion de crear datos. Agregaremos información
Hacemos un select * from customer; y comprobamos que no hay dato todavía
![image](https://user-images.githubusercontent.com/114931679/208472626-60d41641-aa52-4644-b910-fc59e7ad171e.png)

Añadiremos la información
![image](https://user-images.githubusercontent.com/114931679/208475263-a6da35d5-5287-439c-bf0b-1e1c3a975a29.png)
Comprobamos que se ha añadido correctamente a la base de datos
![image](https://user-images.githubusercontent.com/114931679/208475788-99d1e16e-8687-4dc4-a661-73d5d0905735.png)



















