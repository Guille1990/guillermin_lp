# _Guillermin LP_
#### contar palabras

Si necesitas contar el total de palabras contenidas en un fichero de texto solo debes utilizar el comando `contar` de _Guillermin LP_

```shell
$ guill contar fichero_uno.txt
```

La salida de esta instrucción tendrá el siguiente formato:
`[nombre fichero] [numero de palabras]`

```Shell
fichero_uno.txt   3
```

Si necesitas contar las palabras de varios ficheros de texto en una sola ejecución, solo debes agregar los ficheros que requieras separados por una coma `,` a la instrucción `contar`

```shell
$ guill contar fichero_uno.txt,fichero_dos.txt
```

El resultado de dicha ejecución se mostrara en la terminal con el mismo formato mostrado en la ejecución de un solo archivo adicionando un salto de línea por cada fichero solicitado.

```shell
fichero_uno.txt   3
fichero_dos.txt   80
```

#### Generar resumen

Si necesitas generar un resumen de un fichero de texto puedes utilizar la instrucción `resumir` de _Guillermin LP_ indicando después de la palabra reservada `resumir` el nombre del archivo de origen y separado por uno o varios espacios el nombre del archivo de salida que contendrá el resumen requerido.

```Shell
$ guill resumir fichero_origen.txt fichero_salida.txt
```

#### Traducir

Si necesitas traducir  el contenido de un fichero de texto a un idioma especifico puedes utilizar la instrucción `traducir` de _Guillermin LP_ indicando después de la palabra reservada `traducir` el nombre del archivo de origen y separado por uno o varios espacios el nombre del archivo de salida. 

Para indicar el idioma del archivo de origen debes utilizar el flag `--de` asignándole mediante el operador igual `=` el identificador del idioma. 

Para indicar el idioma de salida debes utilizar el flag `--a` asignándole mediante el operador igual `=` el identificador del idioma.

```shell
$ guill traducir fichero_origen.txt fichero_salida.txt --de=es --a=ing
```

#### Generar audio mp3 a partir de un fichero de texto

Si necesitas generar un fichero de audio a partir de un fichero de texto puedes usar la instrucción `audio` de _Guillermin LP_ indicando después de la palabra reservada `audio` el nombre del archivo de origen y separado por uno o varios espacios el nombre del archivo resultante.

```Shell
guill audio fichero_origen.txt fichero_salida.mp3
```