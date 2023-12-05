# Examen Entornos de Desarrollo 
## Tema 3: Git. 05/12/23


Nombre y apellidos: Edgar Fenollar Canto 	 
<br>Fecha: 05/12/2023 

 

LINK DEL REPOSITORIO:________________________________________________ 

> Vamos a crear una primera versión de una calculadora.  
> Debajo de cada ejercicio deberá aparecer capturas de pantalla pertinentes que justifiquen su realización. Intentad hacer todo lo posible desde la consola si no se indica lo contrario. 
> Se valorará negativamente las malas prácticass de GIT 

 

**1.- (0,75) Crea un repositorio en github “AAAExamen23ED“ e invítame a colaborar: "TomBort8" . AAA serán las primeras letras de tu nombre, 1er apellido y 2º apellido respectivamente.** 
<img src="https://i.ibb.co/3kt9wYJ/imagen-2023-12-05-122442366.png">
<img src="https://i.ibb.co/q147PK6/imagen-2023-12-05-122606887.png">

**2.- (0,75) Inicializa el repostiorio en local y vincúlalo al repostiroio de github** <img src="https://i.ibb.co/L0Bc1d1/imagen-2023-12-05-122802722.png">

**3.- Crea un main que pida 2 números por teclado.** 

```
import java.util.Scanner; 

 

public class MostrarNumeros { 

 

    public static void main(String[] args) { 

        Scanner scanner = new Scanner(System.in); 

 

        System.out.println("Por favor, ingresa el primer número:"); 

        double numero1 = scanner.nextDouble(); 

 

        System.out.println("Ahora, ingresa el segundo número:"); 

        double numero2 = scanner.nextDouble(); 

 

        System.out.println("Los números ingresados son:"); 

        System.out.println("Número 1: " + numero1); 

        System.out.println("Número 2: " + numero2); 

 

        scanner.close(); 

    } 

} 
```
> Sube los cambios al repositorio. 

<img src="https://i.ibb.co/WGBFT2G/imagen-2023-12-05-123152420.png">

<img src="https://i.ibb.co/jkXLMdh/imagen-2023-12-05-123526865.png">

<img src="https://i.ibb.co/yNbk0wM/imagen-2023-12-05-123624278.png">

**4.- (0,2) Crea  un fichero ExplicaCalculadora.txt : “Este programa es una calculadora que va a poder realizar las operaciones básicas: sumar, restar, multiplicar y dividir”.** 

<img src="https://i.ibb.co/SNRPNw2/imagen-2023-12-05-123859313.png">

<img src="https://i.ibb.co/Pj7FzW7/imagen-2023-12-05-123931727.png">

*  **4.1  (0,3)Crea también un fichero de texto que no debes subir a github pero debe estar dentro de la carpeta. NoSubir.txt: (Este archivo debes añadirlo y quitarlo, como si te hubieras confundido). “Este archivo debe estar en la carpeta pero no subido a git”.** 

<img src="https://i.ibb.co/9q7X5fx/imagen-2023-12-05-124154303.png">

> Muestra por comandos que no lo has subido 
<img src="https://i.ibb.co/zHwYhjQ/imagen-2023-12-05-124554438.png">

> Sube los cambios al repositorio. 
<img src="https://i.ibb.co/y5K4JQ6/imagen-2023-12-05-124653293.png">
<img src="https://i.ibb.co/n8sf81f/imagen-2023-12-05-124838061.png">
<img src="https://i.ibb.co/L1kdDwD/imagen-2023-12-05-124804164.png">

**5.- (0,5) Muestra la diferencia entre los 2 últimos commits.** 
<img src="https://i.ibb.co/f4zrgmX/imagen-2023-12-05-124954743.png">

**6.- (0,5) Crea 2 ramas SUMADORES y RESTADORES** 
<img src="https://i.ibb.co/pW7FNfm/imagen-2023-12-05-125044674.png">

**7.- Sitúate en SUMADORES y añade al main lo siguiente:**

```
public static double sumar(double a, double b) { 

        return a + b; 

    } 
public static double multiplicar(double a, double b) { 

        return a * b; 

    } 

public static double potencia(double base, double exponente) { 

        return Math.pow(base, exponente); 

    }  
```
<img src="https://i.ibb.co/fvVgJs0/imagen-2023-12-05-125315595.png">
> Sube los cambios al repositorio.
<img src="https://i.ibb.co/hfxTzpp/imagen-2023-12-05-125523671.png">
<img src="https://i.ibb.co/7XjDHcQ/imagen-2023-12-05-125729585.png">

**8.- Sitúate en RESTADORES y añade al main lo siguiente:**

```
public static double restar(double a, double b) { 

        return a - b; 

    } 

public static double dividir(double a, double b) { 

        if (b != 0) { 

            return a / b; 

        } else { 

            throw new IllegalArgumentException("No se puede dividir por cero"); 

        } 

    } 

public static double raizCuadrada(double a) { 

        if (a >= 0) { 

            return Math.sqrt(a); 

        } else { 

            throw new IllegalArgumentException("No se puede calcular la raíz cuadrada de un número negativo"); 

        } 

    } 
```
<img src="https://i.ibb.co/r4B6qDY/imagen-2023-12-05-125919955.png">

> Sube los cambios al repositorio. 
<img src="https://i.ibb.co/D88vbpf/imagen-2023-12-05-130047995.png">
<img src="https://i.ibb.co/FmckGpT/imagen-2023-12-05-130128234.png">

**9.- (1) Muestra la diferencia entre las ramas sumadores y restadores y guárdalo en un fichero llamado DIFERENCIA _RAMAS (desde consola). Este ficehro debe subirse al repositorio.** 

<img src="https://i.ibb.co/yfM5Hj7/imagen-2023-12-05-130501317.png">
<img src="https://i.ibb.co/0V3qfQh/imagen-2023-12-05-130950546.png">
<img src="https://i.ibb.co/23NcFBR/imagen-2023-12-05-131205397.png">
<img src="https://i.ibb.co/x311cjh/imagen-2023-12-05-131258281.png">
 

**10.- (1,5) Fusiónalo en main (consola) y resuelve el conflicto (en gitHUB).** 
<img src="https://i.ibb.co/pv3rnft/imagen-2023-12-05-131630394.png">
<img src="https://i.ibb.co/w7tSjmf/imagen-2023-12-05-131805169.png">
> Sube los cambios al repositorio. 
<img src="https://i.ibb.co/RcrJk9H/imagen-2023-12-05-131940197.png">
<img src="https://i.ibb.co/V2LVf0L/imagen-2023-12-05-132229792.png">
No ha dado ningun conflicto al hacer el push, las ramas se han fusionado correctamente.
 

**11.-(0,5) Borra las ramas SUMADORES Y RESTADORES.**
<img src="https://i.ibb.co/wd4JxQn/imagen-2023-12-05-132357406.png">
 

**12.- (0,5) entra a SOURCETREE y haz una captura del eje temporal del repositorio. Haz una breve explicación de lo que observas.** 
> <img src="https://i.ibb.co/r30qd4j/imagen-2023-12-05-132714973.png">
> Se ve como en el primer punto se crea el MostrarNumeros, el commit del archivo que no hay que subir para probar que no se ha subido, despues se divide en 3 ramas las cuales son SUMADORES y RESTADORES, despues se sube DIFERENCIA_RAMAS.txt, cuando se fucionan las ramas SUMADORES y RESTADORES con el master. Arriba del todo se ve que todavia no se ha echo el commit de la eliminacion de las ramas.
 

**13.- (1) ¿ Cuál es la diferencia entre “git pull” y “git clone” ?** 
> El git pull sirve para actualizar un repositorio sin tener que clonar todos los archivos de nuevo, es decir: Es como hacer un push pero al reves.

> El git clone sirve para clonar un repositorio tal y como esta en github y poder trabajar en el.
 

 

**14.- (1) Abre el main y déjalo inservible. Sube los cambios. Deshaz el último commit.**
<img src="https://i.ibb.co/s1hQHsj/imagen-2023-12-05-133523085.png">
 <img src="https://i.ibb.co/vxP0npt/imagen-2023-12-05-133458877.png">

**15.- (1) Vuelve al estado en el que estaba el proyecto al acabar el ejercicio 3 en local.**
<img src="https://i.ibb.co/R3Z0Zr4/imagen-2023-12-05-133824878.png">
<img src="https://i.ibb.co/bmHBLKn/imagen-2023-12-05-133858842.png">
 
 
 **16.-(0,5) Añade este documento al repoitorio, con todas las imágenes para que se pueda ver desde git.**
<img src="https://i.ibb.co/2SjMt9k/imagen-2023-12-05-134057133.png">

**17.- Por último, ejecutad el siguiente comando:** 

> *history > historial.txt* 

**sube el resultado a aules junto al PDF de este documento.** 