# Estructuras de control
## ¿Qué son?
Se utilizan para cambiar el flujo del programa y conseguir que en ciertos casos se ejecute un trozo de código u otro, dependiendo de lo que se este evaluando.
Estas son:
1. IF
2. ELSE
3. ELSE IF 
   
## IF
Es la estructura de control mas sencilla y se utiliza para que en caso de que se cumpla la sentencia que hay dentro del paréntesis, se ejecute el código que está dentro de las llaves.
Cada vez que se va a evaluar un if, la CPU se para con el fin de comprobar los valores dentro de la sentencia.


```java
public class If {

	public static void main(String[] args) {
		int edad = 0;
		
		if (edad >= 18) {
			System.out.println("Eres mayor de edad");
		}
	}
}

```

## ELSE
Se utiliza cuando la sentencia if anterior no se cumple, entonces se ejecurta el código que hay dentro de las llaves del else.
En este caso, no existen paréntesis, ya que la condición es contraria a la anterior.
Si abusamos del else, o de muchos if con else, lo que conseguiremos es que nuestro código cada vez esté más indentado hacia la derecha haciendolo más complejo de entender a la vez que es un indicativo de que el código que tenemos delante está intentando hacer más cosas de las que debería.

```java
public class If {

	public static void main(String[] args) {
		int edad = 0;
		
		if (edad >= 18) {
			System.out.println("Eres mayor de edad");
		} else {
			System.out.println"Eres menor de edad"();
		}
	}
}

```

## ELSE IF
Se emplea cuando lo que queremos conseguir es evaluar un subconjunto dentro de un conjunto grande.

```java
package estructura_if;

public class If {

	public static void main(String[] args) {
		
		int edad = 16;
		
		if (edad >= 18) {
			System.out.println("Eres mayor de edad");
		} else if (edad  > 15) {
			System.out.println("Estas en pleno pavo");
		} else {
			System.out.println("Eres menor de edad");
		}

	}

}
```

## Clausula de guarda
Es una manera de asegurarnos que el código es válido, es decir, es un if que si se cumple, la ejecución del código no debe seguir.

```java
package estructura_if;

public class If {

	public static void main(String[] args) {
		
		int edad = 16;
		
		if (edad >= 18) {
			System.out.println("Eres mayor de edad");
			return;
		}
			
		System.out.println("Eres menor de edad");	

	}

}
```

## Switch
Es una estructura de control en la que según lo que valga la variable, se ejecutará un código u otro.
Esta estructura no es muy escalable, ya que cada vez que quieras añadir un caso nuevo, tienes que modificarla.
Ejemplo:

```java
public class estructura_switch {

	public static void main(String[] args) {
		int num = 2;
		
		switch (num) {
		case 1:
			System.out.println("El valor es 1");
			break;
		case 2:
			System.out.println("El valor es 2");
			break;
		default:
			System.out.println("El valor es mayor a 2");
			break;
		}

	}

}
```

## OPERADOR TERNARIO
Es equivalente a una sentencia if..else, donde lo primero que se evalua es la sentencia (está antes del interrogante) y los valores de esta sentencia (estan entre :). Si la sentencia es cierta, prevalecerá el valor que esté antes de los :, y si es falsa, la que esté detrás de :.
Ejemplo:

```java
public class estructura_switch {

	public static void main(String[] args) {
		int edad = 2;
		
		String resultado = (edad >= 18) ? "Eres mayor de edad" : "Eres menor de edad";
		System.out.println(resultado);
	}

}
```