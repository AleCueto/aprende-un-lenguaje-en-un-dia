# Aprende un lenguaje de programación en un día (ejercicio voluntario para subir nota).

## Introducción

Cuando te sacaste el carnet de conducir, aprendiste las normas de circulación así como los fundamentos básicos para manejar un coche: volante, marchas, freno, acelerador, embrague, retrovisores... Seguramente, el coche que conduces ahora es diferente al que utilizaste para aprender a conducir, no obstante, lo puedes llevar sin problema. Cada coche tiene sus peculiaridades, pero quien sabe manejar un automóvil, puede adaptarse a las medidas, tacto y comportamiento de un vehículo en cuestión de horas.

Aprender a programar es como aprender a conducir. Si tienes una base sólida de programación y sabes manejar con soltura los tipos de datos, bucles, arrays, clases, métodos, etc. podrás pasar de un lenguaje a otro en un período relativamente corto, simplemente tendrás que adaptarte a la sintaxis y a las peculiaridades del nuevo lenguaje.

Con este ejercicio se pretende despertar el interés por otros lenguajes de programación distintos al que el alumno está estudiando como primer lenguaje.

Sigue los pasos que se indican a continuación.

## Creación del equipo

Este ejercicio se debe hacer en grupos de 3 alumnos. Uno de ellos será el representante del grupo.

## Forkea forkea

El representante del grupo debe hacer un *fork* de este repositorio para utilizarlo como base.

## Añadiendo colaboradores

El encargado del grupo deberá añadir como colaboradores del repositorio *forkeado* a los otros dos miembros, para trabajar todos sobre los mismos archivos. Cuando alguien es colaborador en un repositorio, puede hacer *push* a él sin necesidad de pedir permiso o hacer *pull request*.

Para añadir colaboradores hay que hacer click en la pestaña *Settings* y seleccionar luego *Collaborators* en el menú.

## Miembros del grupo

Escribe aquí los miembros del grupo. El primero es el representante o encargado.

* Alejandro Cueto
* Natalia Castillo
* Joseph Lucas Sanjuan

## Lenguaje de programación

El profesor llevará una cajita llena de papelitos con los nombres de distintos lenguajes de programación. Los encargados de cada grupo meterán la mano en la caja y sacarán dos papelitos, de los cuales el grupo elegirá uno. No se permite hacer intercambio de papelitos entre grupos.

Escribe el lenguaje de programación elegido por el grupo.

* C#

Los papelitos se han recortado de este [documento](lenguajes_de_programacion.pdf).

## Información sobre el lenguaje

C# es un lenguaje desarrollado en el año 2000 por Microsoft. 
Su sintáxis se basa en C/C++-
Su gran ventaja se basa en su uso para la plataforma .NET, también desarrollada por Microsoft.
Aunque se use en .NET C# es un lenguaje independiente, por lo que también se usa para otros propósitos como por ejemplo el desarrollo de videojuegos en el 
game engine unity. 

![imagen](https://user-images.githubusercontent.com/91873580/146737268-9b51e6c4-91f3-4324-8d34-d45d2ef60017.png)
![imagen](https://user-images.githubusercontent.com/91873580/146737392-219e2680-ee52-49d2-b20d-be5cc7f30097.png)


## Herramientas de desarrollo

Vamos a usar Visual Studio Code, al crear un archivo.cs nos dice que necesitamos la extensión C#. 
Luego nos indica que nos falta el paquete de herramientas para C# (Software Development Kit):
Nos descargamos .NET Core SDK desde [aquí](https://dotnet.microsoft.com/en-us/download/dotnet/sdk-for-vs-code)

## Poniendo en práctica el lenguaje

Pon en práctica el lenguaje de programación realizando los siguientes ejercicios. Para cada uno de los ejercicios, pega el código fuente de la solución y una captura de pantalla.

### 1. ¡Hola mundo!

Realiza un programa que muestre por pantalla la frase **¡Hola mundo!**.

```C#
using System;

namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      Console.WriteLine("Hello World!");    
    }
  }
}
```
### 2. Pirámide

Dada una altura introducida por el usuario, realiza un programa que pinte una pirámide a base de asteriscos con la altura indicada.

```C#
using System;

namespace piramide
{
    class Program
{
    static void Main(string[] args)
    {
        int altura = 0;
        int caracteres = 1;
        Console.WriteLine("Vamos a pintar una pirámide!");    
        Console.WriteLine("Introduce la altura!");    
        altura = Convert.ToInt32(Console.ReadLine());
        int espacios = altura;

        for(int i = 0; i < altura; i++){
            PintarEspacio(espacios);
            espacios--;
            PintarCaracter(caracteres);
            caracteres+=2;

            Console.WriteLine();
        }
    }

    private static void PintarCaracter( int caracteres){
        for(int i = 0; i < caracteres; i++){
            Console.Write("*");
        }
    }

    private static void PintarEspacio( int espacios){
        for(int i = 0; i < espacios; i++){
            Console.Write(" ");
        }
    }
}
}
```
### 3. Arrays y números aleatorios

Realiza un programa que rellene un array (o una estructura similar) con 20 números enteros aleatorios entre 1 y 100 y que seguidamente los muestre por pantalla. A continuación, se deben pasar los números primos a las primeras posiciones del array y los no primos a las posiciones restantes. Muestra finalmente el array resultado.

## Presentación de resultados

Los ejercicios que hemos tenido que hacer en C# se nos han hecho realmente sencillos. Esto es porque una vez aprendida la lógica detras de las senctencias básicas (bucles, condiciones arrays...) es la misma a la aprendida en clase y porque la sintáxis de C# a este nivel es muy parecida a la de java (lenguaje estudiado).

## Recompensa

* Todos los alumnos que realicen correctamente la actividad tendrán 0'25 puntos extra en la nota del trimestre.

* Los miembros del equipo más votado ganarán un premio.

:star: Si te ha gustado este ejercicio, dale una estrellita al [repositorio original](https://github.com/LuisJoseSanchez/aprende-un-lenguaje-en-un-dia).

