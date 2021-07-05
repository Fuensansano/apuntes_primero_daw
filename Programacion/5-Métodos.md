## Métodos
Los métodos se utilizan para evitar que tengamos que repetir el código. En este ejemplo, vamos a hacer un ejericio, que lo que haga es imprimir un número determinado de veces distintas frases y vamos utilizando los métodos para refactorizar.

```java
public class Metodos {

 public static void main(String[] args) {
  System.out.println("hola");
  System.out.println("hola");
  System.out.println("hola");
  System.out.println("hola");

  System.out.println("adios");
  System.out.println("adios");
  System.out.println("adios");
  System.out.println("adios");

  System.out.println("hola");
  System.out.println("hola");
  System.out.println("hola");
  System.out.println("hola");


 }
}
```

En esta versión estamos usando métodos para resolver lo que en la versión anterior estabamos escribiendo a mano.

```java
public class Metodos {

 public static void main(String[] args) {
  hola();

  bye();

  hola();

 }

 public static void hola() {
  for (int i = 0; i < 4; i++) {
   System.out.println("hola");
  }
 }

 public static void bye() {
  for (int i = 0; i < 4; i++) {
   System.out.println("bye");
  }
 }
}
```

Esta es la versión optimizada.

```java
public class Metodos {

 public static void main(String[] args) {
  print("hola", 5);
  print("",1);

  print("bye", 6);
  print("",1);

  print("hola", 7);

 }

 public static void print(String mensaje, int repeticiones) {
  for (int i = 0; i < repeticiones; i++) {
   System.out.println(mensaje);
  }
 }
}
```
