---
Create by: Vizuetcf
---

# Lecture 0 - Functions, Variables

## Índex

* Creating Code with Python
* Functions
* Bugs
* Improving Your First Python Program
* Variables
* Comments
* Pseudocode
* Further Improving Your First Python Program
* Strings and Paremeters
* A small problem with quotation marks
* Formatting Strings
* More on Strings
* Integers or int
* Readability Wins
* Float Basics
* More on Floats
* Def
* Returning Values
* Summing Up


## Creating Code with Python

* VS Code is a special type of text editor that is called a compiler. At the top, you’ll notice a text editor and, at the bottom you will see a terminal where you can execute commands.
* In the terminal, you can execute ``code hello.py`` to start coding.
* In the text editor above, you can type ``print("hello, world")``. This is a famous canonical program that nearly all coders write during their learning process.
* In the terminal window, you can execute commands. To run this program, you are going to need to move your cursor to the bottom of the screen, clicking in the terminal window. You can now type a second command in the terminal window. Next to the dollar sign, type ``python hello.py`` and press the enter key on your keyboard.
* Recall, computers really only understand zeros and ones. Therefore, when you run ``python hello.py``, python will interpret the text that you created in ``hello.py`` and translate it into the zeros and ones that the computer can understand.
* The result of running the ``python hello.py`` program is ``hello, world``.
* Congrats! You just created your first program.


## Functions

* Functions are verbs or actions that the computer or computer language will already know how to perform (realizar).

  A function is like an action or a verb that lets you do something in the program, and generally (*generalmente, por lo general, en general*) speaking (*en general, en terminos generales, de forma general*), any language comes with some predetermined set of *functions*-- some very basic actions or verbs that the computer will already know how to do for you, that the language, really, will know how to do for you. The programmer, the human, can use those functions at will to get the computer to do those things.

* In your ``hello.py`` program, the ``print`` function knows how to print to the terminal window.

 It prints whatever it is you want it to print. 

* The ``print`` function takes arguments. In this case, ``"hello, world"`` are the arguments that the ``print`` function takes.

### Argument

* An argument is an input to a function that somehow influences its behavior.

  The people who invented Python, didn't necessarily know what it is you and I are going to want to print to the screen, so they designed this print function using these parentheses with the ability to take as input some string of text, be it in English or any other human language, that is what you want this function ultimately to print onto the screen.
  
  It's showing us ``hello, world`` on the screen.

  *Ejemlos*:

  ```python
  print   #  1
    (Hello, world)   #  2
  ```
    1. Function 
    2. Argument

#### Side (lateral, 'a un' lado) effect (efecto colateral, o secundario)

In programming, the relationship between an *argument* and a *function* is known (conocido) as a side effect, it can be visual or can be an audio. In this case, it's something that appears on the screen and functions, therefore, can indeed have these side effects.

One of the things they can do as this verb or action is to display on the screen as a side effect, something like those words that we wanted:

```bash
hello, world.
```


## Bugs and Debugging (Depuración)

Bugs are a natural part of coding. These are mistakes, problems for you to solve! Don’t get discouraged! This is part of the process of becoming a great programmer.

A bug is a mistake in a program and they can take so many forms. 

* Imagine in our ``hello.py`` program that accidentally typed ``print("hello, world"`` notice that we missed the final ``)`` required by the compiler. If I purposefully make this mistake, you’ll the compiler will output an error in the terminal window!
* Often, the error messages will inform you of your mistake and provide you clues on how to fix them. However, there will be many times that the compiler is not this kind.

### ¿What is debugging?

La depuración es el proceso de encontrar y solucionar errores en el código fuente de cualquier software. Cuando un software no funciona tal y como se espera, los programadores de computadoras estudian el código para determinar por qué ocurren algunos errores. Con este objetivo, los programadores utilizan herramientas de depuración para ejecutar el software en un entorno controlado, comprobar el código paso a paso y analizar y solucionar el error [1].

---

Extraído de: ***[¿Qué es la depuración?](https://aws.amazon.com/es/what-is/debugging/)***
#### ¿Cómo funciona el proceso de depuración?

El proceso de depuración suele requerir los siguientes pasos. 

**Identificación de errores**

Los desarrolladores, los encargados de las pruebas y los usuarios finales informan de los errores que descubren mientras prueban o usan el software. Los desarrolladores localizan la línea exacta de códigos o el módulo de código que causa el error. Esto puede ser un proceso tedioso y que requiere mucho tiempo. 

**Análisis de errores**

Los codificadores analizan el error mediante el registro de todos los cambios de estado del programa y los valores de los datos. También dan prioridad a la corrección de errores en función de su impacto en la funcionalidad del software. El equipo de software también identifica un calendario para la corrección de errores en función de los objetivos y requisitos de desarrollo.

**Corrección y validación**

Los desarrolladores arreglan el error y hacen pruebas para asegurarse de que el software continúa en funcionamiento como se espera. Pueden escribir nuevas pruebas para comprobar si el error se repite en el futuro.

****_Comparación entre la depuración y las pruebas_****

La depuración y las [pruebas](https://aws.amazon.com/blogs/devops/tag/testing/) son procesos complementarios que garantizan que los programas de software funcionen como deben. Después de escribir una sección completa o parte de un código, los programadores realizan pruebas para identificar fallos y errores. Una vez encontrados los errores, los codificadores pueden comenzar el proceso de depuración y trabajar para librar al software de cualquier error.

#### ¿Cuáles son los errores de codificación que se deben depurar?

Los defectos de software surgen debido a la complejidad inherente al desarrollo de software. También se observan pequeños errores de producción después de que el software esté en funcionamiento porque los clientes lo usan de forma inesperada. A continuación, presentamos algunos tipos de errores comunes que suelen requerir el proceso de depuración.

**Errores de sintaxis**

Un error de sintaxis es un fallo que se produce cuando un programa de computación tiene una sentencia mal escrita. Es el equivalente a una errata o error ortográfico en el procesamiento de textos. El programa no se compilará ni se ejecutará si hay errores de sintaxis. El software de edición de código suele resaltar este error.

1. **Errores semánticos**

Los errores semánticos se producen por el uso inadecuado de las declaraciones de programación. Por ejemplo, si traduce la expresión _x_/(2 π) a [Python](https://aws.amazon.com/what-is/python/?trk=faq_card), podría escribir lo siguiente:

_y = x / 2 * math.pi_

Sin embargo, esta declaración no es correcta porque la multiplicación y la división tienen la misma prioridad en Python y se evalúan de izquierda a derecha. Por lo tanto, esta expresión se calcula como (xπ)/2, lo que da lugar a errores.

2. **Errores lógicos**

Los errores lógicos se producen cuando los programadores tergiversan el proceso o el algoritmo de un programa de computación. Por ejemplo, el código puede salir de un bucle demasiado pronto o puede tener un resultado if-then incorrecto. Puede identificar los errores lógicos si recorre el código para varios escenarios diferentes de entrada o salida.

3. **Errores de tiempo de ejecución**

Los errores de tiempo de ejecución se producen debido al entorno informático en el que se ejecuta el código del software. Algunos ejemplos son el espacio de memoria insuficiente o el desbordamiento de la pila. Para resolver los errores de tiempo de ejecución, puede rodear las declaraciones en bloques try-catch o registrar la excepción con un mensaje apropiado.

#### ¿Cuáles son algunas de las estrategias de depuración más comunes?

Hay varias estrategias que los programadores usan para minimizar los errores y reducir el tiempo necesario para la depuración.

1. **Desarrollo incremental de programas**

El desarrollo incremental consiste en desarrollar los programas en secciones manejables, de modo que se prueben con frecuencia pequeñas porciones del código. De este modo, los programadores pueden localizar los errores que encuentren. También les permite trabajar en un error a la vez en lugar de en múltiples errores después de escribir grandes secciones de código.

2. **Rastreo**

El rastreo es un método popular de depuración, sobre todo para los programas más pequeños. Los desarrolladores trabajan hacia atrás desde el lugar donde se produjo un error grave para identificar el punto exacto de aparición en el código. Lamentablemente, el proceso se vuelve más difícil de lograr a medida que aumenta el número de líneas de código.

3. **Depuración remota**

La depuración remota es la depuración de una aplicación que se ejecuta en un entorno distinto al de su máquina local. Por ejemplo, puede usar herramientas de depuración instaladas de forma remota para resolver el error.

4. **Registro**

La mayoría de los programas de computación registran los datos internos y otra información crítica, como el tiempo de ejecución y los estados del sistema operativo, en archivos de registro. Los desarrolladores estudian los archivos de registro para localizar y resolver los errores. También usan herramientas como los analizadores de registros para automatizar el procesamiento de los archivos de registro.   

5. **Depuración en la nube**

La depuración de aplicaciones complejas en la nube es un reto porque los desarrolladores tienen que emular las arquitecturas de la nube en las máquinas locales. Con el tiempo, pueden surgir diferencias de configuración entre el entorno de la nube y el entorno emulado. Esto da lugar a más errores en producción y a ciclos de desarrollo más largos. Se necesitan herramientas especiales para una depuración más eficaz de la nube.

---
## Improving Your First Python Program

* We can personalize your first Python program.
* In our text editor in hello.py we can add another function. input is a function that takes a prompt as an argument. We can edit our code to say

```python

input("What's your name? ")
print("hello, world")

```

* This edit alone, however, will not allow your program to output what your user inputs. For that, we will need to introduce you to variables

### Sintaxis error

When we talk about of a syntax error, which (*que, but not a cuestion*) refers (*que se refuere, que hace referencia a, que hace referencia* ) to my having made a mistake at my keyboard. And this one, is pretty (*bonito, precioso*) straightforward (*sencillo, direc tamente, sin complicaciones*) (*bastante sencllo, bastante directo, bastante claro*). 

  *Ejemplos*:
  ```python
  
  print("Hello, world"  #   1
  
  ```
  ```bash
  
  $ py hello.py

  ## --- ##
  
  $ SyntaxError: '(' was never closed

  ```
  > Closed: *Encerrado, encerrada*
  
  1. It says that this open parenthesis was never closed.
  
  > That's probably pretty intuitive, and i need to do close it. 

---

## Question round

### Quesiton 1

- **AUDIENCE**: Could I write code inside a word or, for example, Microsoft Excel? And what's the barrier to doing that? 

- **DAVID MALAN**: A really good question, and allow me to very explicitly say to the entire internet that you should not write code with Microsoft Word. I mentioned that only because it's a tool via which you can write text and code is, at the end of the day, just text. But it's not the right tool for the job. We don't need bold facing, underlining, paragraphs and the like. We generally want something much simpler than Microsoft Word or Google Docs. And so VS Code is an example of just a more general purpose text editor. Its purpose in life is to allow you, the human, to edit text. Nowadays these text editors come with many more features. In fact, you'll notice that even in my code here, even though it's just one line, there's a bit of color to it. The word "print" for me is appearing in blue. The parentheses are black. And we'll see as we write more lines of code, more and more of the lines will come to life in various colors.

- Now that's just one feature of a text editor. We'll see too that it has features like this built-in terminal window. It's going to have a built-in tool for debugging or finding problems with code. And it's just a very popular tool nowadays, but there are many, many others out there. You're welcome to use them for this course and beyond. We just happen to use this one in large part too because you can also use VS Code nowadays for free in the cloud. How about one other question here on programming with Python or hello, world or syntax more generally? 


### Question 2

- **AUDIENCE**: Yeah I was trying to ask if it's not possible to run the computer using the terminal window? 

- **DAVID MALAN**: I think I heard is it not-- if it's possible to run the program without the terminal window? Are you-- 

- **AUDIENCE**: Yes, sir. 

- **DAVID MALAN**: OK, you froze for me again. But let me infer what the question is. So in this environment, as I've configured my computer, I can only run these Python programs via the terminal window. Now that's good for me, the programmer, or the person who's trying to learn how to program, but it's not very good if you want to ship this software and have other people use your actual code. You can absolutely write programs and then allow other people to use, not a command line interface, but a graphical user interface or GUI-- G-U-I. 
- This is just one mechanism and perhaps(*talvez, eventualmente*), I think, the best one with which to start writing code because eventually it's going to give us a lot more control. 

---

## Return values

I can write the next code in vsc:

```python
Input("What's your name?")
print("My namje is Fernando")
```

Wen we run that code in the terminal, we can note a mistake, that code obtain just one output:

```bash
py hola_mundo.py

My name is <name>
```

### Variables

To solved that problem, we need know the concept of ***Variable***.

> A variable is just a container for a value within (*en*, *dentro de*, *en la direccion*) your own program.

* In your program, you can introduce your own variable in your program by editing it to read.

```python
name = input("What's your name? ")
print("hello, world")
```
  Notice that this equal = sign in the middle of name = input("What's your name? ") has a special role in programming. This equal sign literally assigns what is on the right to what is on the left. Therefore, the value returned by input("What's your name? ") is assigned to name.

* If you edit your code as follows, you will notice an error

```python 
name = input("What's your name? ")
print("hello, name")
```

* The program will return hello, name in the terminal window regardless of what the user types.
* Further editing our code, you could type

```python 
name = input("What's your name? ")
print("hello,")
print(name)
```

* The result in the terminal window would be

```shell
What's your name? David
hello
David
```

* We are getting closer to the result we might intend!
* You can learn more in Python’s documentation on [data types](https://docs.python.org/3/library/datatypes.html).

---

## Comments and Pseudocode
### Comments

Comments are notes to yourself in your code and you include comments by way of a special symbol-- **in Python it's going to be the *hash* symbol, typically**-- and that allows you to write the equivalent of a note to yourself but in a way that's not going to break your code. The computer actually ignores your comment. It's just there for you, it's just there for your teacher, it's just there for your colleague with whom (*que*, *a quien*, *quien*, *cuyo*) you're sharing ultimately that code.

* Comments are a way for programmers to track what they are doing in their programs and even inform others about their intentions for a block of code. In short, they are notes for yourself and others that will see your code!
* You can add comments to your program to be able to see what it is that your program is doing. You might edit your code as follows:

```python
# Ask the user for their name
name = input("What's your name? ")

# Say hello to user
print("hello,")
print(name)
```

* Comments can also serve as to-do list for you.

> So this isn't really necessary for a program this small. It's pretty obvious with just one or two or three lines what the program is doing. It's just as fast to read the code than the comments, but getting into this habit is generally a good thing-- to comment your code every one or a few lines so as to remind yourself and others what it is your intent and your code is doing. What's nice about comments too is this-- comments can also serve to be sort of a to-do list for yourself.
### Pseudocode 

Pseudocode isn't a formal thing. It's not one specific language. It's just using English or your own human language to express your thoughts succinctly, methodically, algorithmically, so to speak. 
It just kind (*tipo*) of allows (*permite*, *permite a*) (nos permite) you to outline (esbozar) your program even (*incluso*, *hasta*) in advance (*avance*, *avanzar*, *adelantas*, *anticipar*).

* Pseudocode is an important type of comment that becomes a special type of to-do list, especially when you don’t understand how to accomplish a coding task. For example, in your code, you might edit your code to say:

```python
# Ask the user for their name   #  1
name = input("What's your name? ")

# Print hello   #  1
print("hello,")

# Print the name inputted   #  1
print(name)

'''
This is a comment, i can write some lines
whith that form
'''   #  2

```
	1. Pseudocode, it´s like a to-do list, whith this, i can think about of what i can do tomorrow.
	2. alternative form to do comments.

# Multiple Function Arguments

## Further Improving Your First Python Program

* We can further edit our code as follows:

```python
# Ask the user for their name
name = input("What's your name? ")

# Print hello and the inputted name
print("hello, " + name)
```

* It turns out that some functions take many arguments.
We can use a comma ``,`` to pass in multiple arguments by editing our code as follows:

```python
# Ask the user for their name
name = input("What's your name? ")

# Print hello and the inputted name
print("hello,", name)
```

* The output in the terminal, if we typed “David” we would be ``hello, David``. Success.


## Strings and Paremeters

* A string, known as a ``str`` in Python, is a sequence of text.
`* Rewinding a bit in our code back to the following, there was a visual side effect of having the result appear on multiple lines:

```python
# Ask the user for their name
name = input("What's your name? ")
print("hello,")
print(name)
```

* Functions take arguments that influence their behavior. If we look at the documentation for ``print`` you’ll notice we can learn a lot about the arguments that the print function takes.
* Looking at this documentation, you’ll learn that the print function automatically include a piece of code ``end='\n'. This`` \n ``indicates that the print function will automatically create a line break when run. The print function takes an argument called `` end` and the default is to create a new line.
* However, we can technically provide an argument for ``end`` ourselves such that a new line is not created!
* We can modify our code as follows:

```python
# Ask the user for their name
name = input("What's your name? ")
print("hello,", end="")
print(name)
```
  By providing ``end=""`` we are over-writing the default value of ``end`` such that it never creates a new line after this first print statement. Providing the name as “David”, the output in the terminal window will be ``hello, David``.

* Parameters, therefore, are arguments that can be taken by a function.
* You can learn more in Python’s documentation on [``print``](https://docs.python.org/3/library/functions.html#print).


## A small problem with quotation marks

* Notice how adding quotation marks as part of your string is challenging.
* ``print("hello,"friend"")`` will not work and the compiler will throw an error.
* Generally, there are two approaches to fixing this. First, you could simply change the quotes to single quote marks.
* Another, more commonly used approach would be code as ``print("hello, \"friend\"")``. The backslashes tell the compiler that the following character should be considered a quotation mark in the string and avoid a compiler error.


## Formatting Strings

* Probably the most elegant way to use strings would be as follows:

```python
# Ask the user for their name
name = input("What's your name? ")
print(f"hello, {name}")
```
  Notice the ``f`` in ``print(f"hello, {name}")``. This ``f`` is a special indicator to Python to treat this string a special way, different than previous approaches we have illustrated in this lecture. Expect that you will be using this style of strings quite frequently in this course.


## More on Strings

* You should never expect your user will cooperate as intended. Therefore, you will need to ensure that the input of your user is corrected or checked.
* It turns out that built into strings is the ability to remove whitespace from a string.
* By utilizing the method ``strip`` on ``name`` as ``name = name.strip()``, it will strip all the whitespaces on the left and right of the users input. You can modify your code to be:

```python
# Ask the user for their name
name = input("What's your name? ")

# Remove whitespace from the str
name = name.strip()

# Print the output
print(f"hello, {name}")
```
  Rerunning this program, regardless of how many spaces you type before or after the name, it will strip off all the whitespace.

* Using the ``title`` method, it would title case the user’s name:

```python
# Ask the user for their name
name = input("What's your name? ")

# Remove whitespace from the str
name = name.strip()

# Capitalize the first letter of each word
name = name.title()

# Print the output
print(f"hello, {name}")
```

* By this point, you might be very tired of typing ``python`` repeatedly in the terminal window. You cause us the up arrow of your keyboard to recall the most recent terminal commands you have made.
* Notice that you can modify your code to be more efficient:

```python
# Ask the user for their name
name = input("What's your name? ")

# Remove whitespace from the str and capitalize the first letter of each word
name = name.strip().title()

# Print the output
print(f"hello, {name}")
```
  This creates the same result as your previous code.

* We could even go further!

```python
# Ask the user for their name, remove whitespace from the str and capitalize the first letter of each word
name = input("What's your name? ").strip().title()

# Print the output
print(f"hello, {name}")
```

* You can learn more about strings in Python’s documentation on [``str``](https://docs.python.org/3/library/stdtypes.html#str)


## Integers or int

In Python, an integer is referred to as an int.
In the world of mathematics, we are familiar with +, -, *, /, and % operators. That last operator % or modulo operator may not be very familiar to you.
You don’t have to use the text editor window in your compiler to run Python code. Down in your terminal, you can run python alone. You will be presented with >>> in the terminal window. You can then run live, interactive code. You could type 1+1 and it will run that calculation. This mode will not commonly be used during this course.
Opening up VS Code again, we can type code calculator.py in the terminal. This will create a new file in which we will create our own calculator.
First, we can declare a few variables.

x = 1
y = 2

z = x + y

print(z)
Naturally, when we run python calculator.py we get the result in the terminal window of 3. We can make this more interactive using the input function.

x = input("What's x? ")
y = input("What's y? ")

z = x + y

print(z)
Running this program, we discover that the output is incorrect as 12. Why might this be?
Prior, we have seen how the + sign concatenates two strings. Because your input from your keyboard on your computer comes into the compiler as text, it is treated a string. We, therefore, need to convert this input from a string to an integer. We can do so as follows:

x = input("What's x? ")
y = input("What's y? ")

z = int(x) + int(y)

print(z)
The result is now correct. The use of int(x), is called “casting” where a value is temporarily changed from one type of variable (in this case a string) to another (here, an integer).

We can further improve our program as follows:

x = int(input("What's x? "))
y = int(input("What's y? "))

print(x + y)
This illustrates that you can run functions on functions. The most inner function is run first, and then the outer one is run. First, the input function is run. Then, the int function.

You can learn more in Python’s Documenation of int.


## Readability Wins

When deciding on your approach to a coding task, remember that one could make a reasonable argument for many approaches to the same problem.
Regardless of what approach you take to a programming task, remember that your code must be readable. You should use comments to give yourself and others clues about what your code is doing. Further, you should create code in a way that is readable.


## Float Basics

A floating point value is a real number that has a decimal point in it, such as 0.52.
You can change your code to support floats as follows:

x = float(input("What's x? "))
y = float(input("What's y? "))

print(x + y)
This change allows your user to enter 1.2 and 3.4 to present a total of 4.6.

Let’s imagine, however, that you want to round the total to the nearest integer. Looking at the Python documentation for round you’ll see that the available arguments are round(number[n, ndigits]). Those square brackets indicate that something optional can be specified by the programmer. Therefore, you could do round(n) to round a digit to its nearest integer. Alternatively, you could code as follows:

# Get the user's input
x = float(input("What's x? "))
y = float(input("What's y? "))

# Create a rounded result
z = round(x + y)

# Print the result
print(z)
The output will be rounded to the nearest integer.

What if we wanted to format the output of long numbers? For example, rather than seeing 1000, you may wish to see 1,000. You could modify your code as follows:

# Get the user's input
x = float(input("What's x? "))
y = float(input("What's y? "))

# Create a rounded result
z = round(x + y)

# Print the formatted result
print(f"{z:,}")
Though quite cryptic, that print(f"{z:,}") creates a scenario where the outputted z will include commas where the result could look like 1,000 or 2,500.


## More on Floats

How can we round floating point values? First, modify your code as follows:

# Get the user's input
x = float(input("What's x? "))
y = float(input("What's y? "))

# Calculate the result
z = x / y

# Print the result
print(z)
When inputting 2 as x and 3 as y, the result z is 0.6666666666 seemingly going on to infinite as we might expect.

Let’s imagine that we want to round this down, we could modify our code as follows:

# Get the user's input
x = float(input("What's x? "))
y = float(input("What's y? "))

# Calculate the result and round
z = round(x / y, 2)

# Print the result
print(z)
As we might expect, this will round the result to the nearest two decimal points.

We could also use fstring to format the output as follows:

# Get the user's input
x = float(input("What's x? "))
y = float(input("What's y? "))

# Calculate the result
z = x / y

# Print the result
print(f"{z:.2f}")
This cryptic fstring code displays the same as our prior rounding strategy.

You can learn more in Python’s documentation of float.


## Def

Wouldn’t it be nice to create our own functions?
Let’s bring back our final code of hello.py by typing code hello.py into the terminal window. Your starting code should look as follows:

# Ask the user for their name, remove whitespace from the str and capitalize the first letter of each word
name = input("What's your name? ").strip().title()

# Print the output
print(f"hello, {name}")
We can better our code to create our own special function that says “hello” for us!

Erasing all our code in our text editor, let’s start from scratch:

name = input("What's your name? ")
hello()
print(name)
Attempting to run this code, your compiler will throw an error. After all, there is no defined function for hello.

We can create our own function called hello as follows:

def hello():
    print("hello")


name = input("What's your name? ")
hello()
print(name)
Notice that everything under def hello() is indented. Python is an indented language. It uses indentation to understand what is part of the above function. Therefore, everything in the hello function must be indented. When something is not indented, it treats it as if it is not inside the hello function. Running python hello.py in the terminal window, you’ll see that your output is not exactly as you may want.

We can further improve our code:


# Create our own function
def hello(to):
    print("hello,", to)


# Output using our own function
name = input("What's your name? ")
hello(name)
Here, in the first lines, you are creating your hello function. This time, however, you are telling the compiler that this function takes a single parameter: a variable called to. Therefore, when you call hello(name) the computer passes name into the hello function as to. This is how we pass values into functions. Very useful! Running python hello.py in the terminal window, you’ll see that the output is much closer to our ideal presented earlier in this lecture.

We can change our code to add a default value to hello:

# Create our own function
def hello(to="world"):
    print("hello,", to)


# Output using our own function
name = input("What's your name? ")
hello(name)

# Output without passing the expected arguments
hello()
Test out your code yourself. Notice how the first hello will behave as you might expect and the second hello, which is not passed a value, will by default output hello, world.

We don’t have to have our function at the start of our program. We can move it down, but we need to tell the compiler that we have a main function and we have a separate hello function.

def main():

    # Output using our own function
    name = input("What's your name? ")
    hello(name)

    # Output without passing the expected arguments
    hello()


# Create our own function
def hello(to="world"):
    print("hello,", to)
This alone, however, will create an error of sorts. If we run python hello.py nothing happens! The reason for this is that nothing in this code is actually calling the main function and bringing our program to life.

The following very small modification will call the main function and restore our program to working order:

def main():

    # Output using our own function
    name = input("What's your name? ")
    hello(name)

    # Output without passing the expected arguments
    hello()


# Create our own function
def hello(to="world"):
    print("hello,", to)


main()


## Returning Values

You can imagine many scenarios where you don’t just want a function to perform an action, but also to return a value back to the main function. For example, rather than simply printing the calculation of x + y, you may want a function to return the value of this calculation back to another part of your program. This “passing back” of a value we call a return value.
Returning to our calculator.py code by typing code calculator.py. Erase all code there. Rework the code as follows:

def main():
    x = int(input("What's x? "))
    print("x squared is", square(x))


def square(n):
    return n * n


main()
Effectively, x is passed to square. Then, the calculation of x * x is returned back to the main function.


## Summing Up

Through the work of this single lecture, you have learned abilities that you will use countless times in your own programs. You have learned about…

* Creating your first programs in Python;
* Functions;
* Bugs;
* Variables;
* Comments;
* Pseudocode;
* Strings;
* Parameters;
* Formatted Strings;
* Integers;
* Principles of readability;
* Floats;
* Creating your own functions; and
* Return values.


---

# Bibliografía

> ***Course links***
> 
> * [Week 0 Functions](https://cs50.harvard.edu/python/2022/weeks/0/)
> * [Lecture 0](https://cs50.harvard.edu/python/2022/notes/0/)
> * [Transcript](https://cdn.cs50.net/python/2022/x/lectures/0/lang/en/lecture0.txt)
> * [Gradebook](https://cs50.me/cs50p)
> 
> ***External links***
> 
> 1. [¿Qué es la depuración](https://aws.amazon.com/es/what-is/debugging/)
> * 