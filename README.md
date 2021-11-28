# Piramide de letras

Es un ejercicio simple en el que se busca crear una piramide que se forma con letras. Lo cree completamente en POO.

## Archivo main.py

Es el archivo principal, donde se llaman los metodos necesarios para que funcione todo.

## Archivo piramide.py

Aqui estan todos los metodos de los cuales "**tipo_letras**" y "**pisos_letras**", son unicamente para que el usuario pueda ingresar valores para que construya la piramide a gusto. Luego tenemos el metodo "contruir" que se ocupa de la logica necesaria para crear dicha piramide. Por ultimo el metodo "__init__" donde se llaman a los metodos "**tipo_letras**" y "**pisos_letras**" para instanciar.

Si no quisieramos los metodos "**tipo_letras**" y "**pisos_letras**", le pasamos los parametros en el metodo constructor, o sea, "__init__" separados por comas, luego del self.

### Metodo _**construir( )**_
Este metodo se ocupa de la logica, tiene 2 ciclos foranidados. El primero se ocupa de iterar para tener la cantidad de pisos. El segundo ciclo se ocupa de iterar sobre la cantidad de letras que va a tener cada piso.

- Funcion _**chr()**_
Esta funcion tomara como argumento un numero y devolverá el carácter asociado a un código ASCII.

- Parametro _**self.num**_ dentro del metodo construir
Si self.num esta en el primer for, se repite solo la letra por fila.
Si self.num esta en el segundo for, se imprimen las letras seguidas.

### Metodo _**inversa( )**_

Simplemente es la misma logica que la funcion anterior pero el segundo ciclo tiene el rango cambiado para que resulte una piramide invertida.

### Metodo _**asteriscos( )**_
La idea es formar una piramide solo con asteriscos.

### Metodo _**asteriscos_invertido( )**_
Para crear la version invertida de la piramide creada con asteriscos.

### Metodo  _**tipo_letras( )**_
Si mecesitamos las letras sean **mayusculas** tendremos que instanciar "self.num" en 65, por otro lado si quisieramos que fuese en **minusculas** deberia instanciar en 97. Este metodo nos da facilidad para hacer esto.

### Metodo _**pisos_letras( )**_
Simplemente lo usamos para saber que altura tendra nuestra piramide.