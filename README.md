# Amo los argumentos
Este repositorio contiene todo el Reto 9.
### 1. De los retos anteriores selecione 3 funciones y escribalas en forma de lambdas.
   * La primera función lambda que creé fue una para desarrollar el punto 3 del Reto #6: "Diseñe una función que calcule la cantidad de carne de aves en kilos si se tienen N gallinas, M gallos y K pollitos cada uno pesando 6 kilos, 7 kilos y 1 kilo respectivamente."
     Aquí, definí una función main y dentro de ella cree una función lambda que me incluyera las variables de la cantidad de pollitos(K), gallos(M) y gallinas(N). El resultado que arrojaría la función sería la cantidad de gallinas multiplicadas por 6, más la cantidad de gallos multiplicados por 7 y eso, más la cantidad de pollitos. Al final, definí la variable resultado como la función lambda e imprimí esa variable resultado.

     ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/d82c34eb-1a00-43ff-b81f-a02796e7a191)

   * La segunda función lambda que creé fue una para desarrollar el punto 4 del Reto #6: "Mi mamá me manda a comprar P panes a 300 cada uno, M bolsas de leche a 3300 cada una y H huevos a 350 cada uno. Hacer un programa que me diga las vueltas (o lo que quedo debiendo) cuando me da un billete de B pesos."
      Primero, definí la función main, luego, dentro de esta función definí la función lambda con el nombre de calcular_vueltas y tomé los argumentos de P (cantidad de panes), M (cantidad de bolsas de leche), H (cantidad de huevos) y B(el valor del billete con el que pagó); asimismo, definí la expresión de la función como el valor del billete menos la suma de las cantidades de cada cosa multiplicadas por su respectivo valor. También puse dos condicionales para que, en el caso de que quedara debiendo la persona, le arroje el mensaje de cuánto queda debiendo, pero, en el valor absoluto de la cantidad que debe y que arroja como resultado la función lambda; si la persona no queda debiendo, el algorimo le arrojará el valor de cuánto queda debiendo.

     ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/611c553e-7cf6-42fc-9bdd-4acd9a39ed15)

   * La tercera función lambda que creé fue una para desarrollar el punto 5 del Reto #6: "Haga un programa que utilice una función para calcular el valor de un préstamo C usando interés compuesto del i por n meses."
     Primero, definí la función main, luego, dentro de esta función definí la función lambda con el nombre de valor_prestamo y tomé los argumentos de c (valor del préstamo), i (porcentaje de interés anual) y n (tiempo que dura la inversión). El resultado o la expresión que arroja esta función es igual a la multiplicación de c por (1+(1/100))^2. Al final, volví a nombrar la función, más, la mencioné con una variable (valor_final_prestamo) y con print, el algoritmo imprime el valor final del préstamo.

     ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/a46c5bf6-54ca-4637-bc05-3c60ad2a3de4)

### 2. De los retos anteriores selecione 3 funciones y escribalas con argumentos no definidos (*args).
   * Para la primera función, seleccioné el punto 7 del Reto #6, el cual, en una de las funciones, se pide calcular el promedio de 5 números, para eso, yo simplemente definí la función para calcular el promedio, pero, en vez de nombrar las variables, puse "*args", así, la función va ir a a la función main para sacar toda la información y realizar los procedimientos con esos procedimientos. El resto simplemente fue lo de siempre, definir una función main y dentro de ella los argumentos (a, b, c, d y e), así como la variable que menciona la función para calcular el promedio.
   
   ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/ac2adb64-e772-417d-8a1b-21f2140d48a0)

   * Para la segunda función, tomé el punto 6 del Reto #6: "El número de contagiados de Covid-19 en el país de NuncaLandia se duplica cada día. Hacer un programa que diga el número total de personas que se han contagiado cuando pasen D días a partir de hoy, si el número de contagiados actuales es C.". Este código es un programa que calcula el número de personas contagiadas en un día futuro "d" basado en el número de contagiados actuales "c". El programa realiza lo siguiente: 1. Define una función calcular_numero_contagiados_dia_d(c, d) que toma dos argumentos: el número actual de contagiados (c) y la cantidad de días en el futuro (d); sin embargo, estos argumentos no se mencionan directamente en la función, sino que se les llama "*args". 2. Calcula el número de contagiados proyectado en el día "d" utilizando la fórmula c * 2 ** d y lo devuelve como un número entero. 3. En el programa principal (bloque if __name__ == "__main__":), el usuario ingresa el número actual de contagiados (c) y la cantidad de días en el futuro (d). 4. Llama a la función calcular_numero_contagiados_dia_d(c, d) con los valores ingresados por el usuario. 5. Muestra el resultado que informa al usuario sobre el número proyectado de contagiados en el día "d" utilizando la fórmula calculada.
   
   ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/496f6d8a-e328-4beb-8568-0a36953a90f4)

   * Para la tercera función, me basé en el punto 1 del Reto #10, el cual, era básicamente calcular el promedio de un arreglo de reales. Mi yo del pasado lo puede explicar mejor: "Cree una lista de números reales y mediante la función "promedioArreglo", inicialicé la variable suma como 0 y dejé que se actualizara a partir de cada elemento que se encontraba en la lista; para que cogiera cada elemento el algoritmo, utilice "for", así, después de que recorra todos los elementos de la lista, esa suma se va a dividir entre la longitud de la lista o la cadena, la cual, hace referencia a la cantidad de elementos presentes en la lista." (Yo, el viernes 13 programando :)). Sin embargo, mi yo del pasado no había descubierto la maravilla de los argumentos para ahorrarse mencionar las variables que iba a utilizar en las funciones, así que, mi yo del futuro cambió eso, me sentí como si hubiera tenido un glow up en programación al hacer eso.

     ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/b86e41a7-7867-40c0-bb7b-15d7c0d8462d)
   
### 3. Escriba una función recursiva para calcular la operación de la potencia.
   El código proporciona una función recursiva llamada potencia_recursiva que calcula la potencia de un número (num) elevado a un exponente (exponente). La función maneja casos base (cuando el exponente es 0, en cuyo caso retorna 1) y realiza llamadas recursivas a la misma función para calcular la potencia en otros casos. El programa principal le pide al usuario la base y el exponente, llama a la función, y luego muestra el resultado calculado, incluyendo la base, el exponente y el resultado de la potencia. En resumen, el código permite calcular potencias de forma recursiva.
   
   ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/8c8a2aea-6fbe-4f44-911e-5c0c522d13f3)

### 4. Utilice la siguiente plantilla de code para contar el tiempo:
   ```python
   import time

    start_time = time.time()
    # instrucciones sobre las cuales se quiere medir tiempo de ejecución
    end_time = time.time()

    timer = end_time - start_time
    print(timer)
   ```
Este código calcula el número de Fibonacci para un valor específico (yo lo tomé como 19), además, utilicé dos enfoques: recursión e iteración. Mide el tiempo que cada enfoque tarda en ejecutarse y muestra los resultados junto con el tiempo de ejecución. La diferencia de tiempo se vuelve significativa a medida que el valor de entrada (n) aumenta, ya que la recursión se vuelve mucho más lenta debido a la sobrecarga de llamadas recursivas a la función, de hecho, puse el 333 y se quedó ahí un mbuen tiempo: mientras que la iteración es más eficiente. Finalmente, se puede ajustar el valor de n para observar esta diferencia en el tiempo de ejecución.
   
   ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/f4e6313a-10aa-4f0c-84a1-35a92c626136)

### 5. Crear cuenta en stackoverflow y adjuntar imagen en el repo
   
   ![image](https://github.com/Cate1911/Los_lambda/assets/141857246/66719575-8940-4923-8a21-f08bb287e3bb)

### 6. Cosas de adultos....ir a linkedin y crear perfil....NO IMPORTA que estén iniciando, si tienen tiempo para redes poco útiles como fb, insta, o tiktok tienen tiempo para crear un perfil mamalón. Dejar enlace en el repo.
 Mi perfil de Linkedin: https://www.linkedin.com/in/caterin-sierra-huertas-27700b297
