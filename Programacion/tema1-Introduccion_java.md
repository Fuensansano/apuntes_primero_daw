# 
## ¿Qué es Java?
1.  lenguaje de programación multiplataforma, es decir, se puede ejecutar un programa java en cualquier entorno (Windows, Linux, Android).
2.  Orientado a objetos y que se complementa con el paradigma de la programción funcional.
3. Es un lenguaje seguro.
4. Multihilo, es decir, un programa puede trabajar en paralelo, puede hacer varias cosas a la vez.
   
## ¿Cómo funciona?
ficheros de código fuente.....pasan por el compilador (javac) y los covierte en ficheros .class.

*Los ficheros .class* son ficheros ejecutables

## Ejemplo practico

Creo un fichero `HelloWorld.java` en el escritorio.
para ello, utilizaremos el siguiente comando:
```shell
nano HelloWorld.java
```
Y escribiremos en el fichero lo siguiente.
```java
public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hola Mundo");
    }
}
```
Para poder compilar este fichero lo que haremos será abrir una terminal teniendo ya instalado el JDK de java.

Para ejecutar el programa en la terminal, seguiriamos los siguientes paso, escribiendo las siguientes líneas por orden en dicha terminal.

```shell
javac HelloWorld.java
```
De esta forma, se compila el código fuente y esto genera el fichero `HelloWorld.class`.

Para poder ejecutarlo, escribiriamos lo siguiente

```shell
java HelloWorld
```
Aquí no haría falta poner la extensión del fichero, porque el interprete de java ya sabe que es `.class`.
