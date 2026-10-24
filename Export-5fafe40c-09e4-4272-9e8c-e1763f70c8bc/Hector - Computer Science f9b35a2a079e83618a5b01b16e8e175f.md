# Hector - Computer Science

[Meet](https://meet.google.com/yso-uppm-ajo?authuser=0)

---

---

[Ejercicios](Hector%20-%20Computer%20Science/Ejercicios%202e235a2a079e83b58e750152e8fa8b44.md)

### Año pasado

A las **funciones** que están dentro de una clase se les llama **métodos** (siempre llevan el self como primer parámetro)

RGB

00000000, 00000000, 00000000 → 1B por color → 3B

16,16,16

256,256,256

2^8  = 256, exponente = n de bits

11111111, 000000000001, 00000000

255 = 0xFF

img : 90X68 (columnas x filas)

vector_imagen[68][90] (filas, cols)

### **Cuantos bits necesito para tener una precisión de 20 millones de colores**

2^x ≥ 20 milloness

10110101010100110100101010101010101010101010101010 → PDF 

SVG

_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _  = RGB

0 0 0 0 00 0 0 00 0 0 0 00 0 0 0 00 0 0 0 0 0 0 0 

0001

FILE SIZE = FILAS X COLUMAS (X N COLOR DEPTH)

[Trading - Opciones y Futuros | CNMV](Hector%20-%20Computer%20Science/Trading%20-%20Opciones%20y%20Futuros%20CNMV%20c4035a2a079e82fdb36601bbc4742ee9.md)

![Untitled](Hector%20-%20Computer%20Science/Untitled.png)

## Ejercicios de binario

**what is the range os possible numbers, in denary from smaller to biggest that can be represented in a one byte binary number when using unseigned binary number**

A byte is composed of 8 bits. When using unsigned binary numbers, the range of possible numbers that can be represented by a one byte binary number is from 0 to 255 (2^8 - 1), where 0 represents the smallest number and 255 represents the largest number.

In binary, the smallest number that can be represented using 8 bits is 00000000, which is equivalent to 0 in denary. The largest number that can be represented using 8 bits is 11111111, which is equivalent to 255 in denary.

Therefore, the range of possible numbers, in denary, from smaller to biggest that can be represented in a one byte binary number when using unsigned binary number is 0 to 255.

**what is the range os possible numbers, in denary from smaller to biggest that can be represented in a one byte binary number when using two’s complemetn**

When using two's complement signed numbers, the range of possible numbers that can be represented by a one byte binary number is from -128 to 127. This is because the most significant bit (MSB) of a one byte two's complement number is used to indicate the sign of the number.

If the MSB is 0, the number is positive and is represented as usual using binary notation. For example, the binary number 01100101 represents the denary number 101.

If the MSB is 1, the number is negative and is represented by taking the two's complement of the absolute value of the number. To take the two's complement, the bits are inverted (i.e., 0s become 1s and 1s become 0s) and 1 is added to the result. For example, to represent -27 using one byte two's complement notation, we start by representing the absolute value of 27 in binary, which is 00011011. Then, we invert the bits to get 11100100 and add 1 to get the two's complement representation of -27, which is 11100101.

Therefore, the range of possible numbers, in denary, from smaller to biggest that can be represented in a one byte binary number when using two's complement signed numbers is -128 to 127.

# EJERCICIO 1 - Pag. 43

1. `biggest = num` y no al revés, estaríamos modificando el input del usuario y no actualizando el mayor
2. OUTPUT tiene que estar fuera del bucle pq no estaríamos enseñando el máximo de todos
3. UNTIL count ≤ 10 pq estaríamos solo pidiendo 9 números en lugar de 10

## Ej 2

1. `total = 0` syntax error, solo 1 = por que es asignación, 2= son comparación
2. `total += marks[index]` run-time error, debden de sumarse en este caso, saldría el último valor del vector que es el que almacena.Homeworks
3. `print(total)` ya que el programa no hace nada sin ese print          

why are logical the most difficult to find? al ejecutar no se muestra ningún error tienes que ser tú con la ayuda de un debugger el que investigues linea a linea                      

## Ej 3

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  

|  | A | B | C | D (average=6) |
| --- | --- | --- | --- | --- |
| Normal | 10 | 30 | 20 | 6 |
| Boundary | 0 , 100 | 0, 70-80 | 9 | 2 , 85 |
| Erroneous | -5, 150 | 120 | 5 | x < 0 |

## Ej 4

1. a = 0
2. a*c > b**2 ⇒ no existen raíces cuadradas negativas

## Ej 6

```diff
IF score > 70 THEN
 OUTPUT "expert"
ELSE IF score < 30 THEN
 OUTPUT "beginner"
ELSE 
 OUTPUT "cadet"
END IF
```

![Untitled](Hector%20-%20Computer%20Science/Untitled%201.png)

# Advent of code

[Advent of Code](https://adventofcode.com/)

1. Lectura de ficheros
2. Manejo de estructuras de datos
    1. listas
    2. pilas
    3. mapas/diccionarios { }
    4. Manejo de la clase string
3. un poquito… de Clases…

```python
def read_file() -> list:
	with open('X') as f:
		return [line.rstrip() for line in f]

### TE PONGO LA CLASE DE HOY

puntos={
    'X' : 1,
    'Y' : 2,
    'Z' : 3
}
cont_puntos=0
def read_file() -> list:
	with open('input2.txt') as f:
		return [line.rstrip() for line in f]

data = read_file()

empates = ['A X','B Y', 'C Z']
ganar = ['A Z', 'B Z', 'C Y']
# perder = ['', 'B Z', 'C X']

for partida in data:
    letra_derecha=partida.split(' ')[1]
    print('letra derecha ', letra_derecha, puntos.get(letra_derecha))
    cont_puntos += puntos.get(letra_derecha)
    
    if partida in empates:
        print(partida + ' ', partida in empates)
        cont_puntos += 3

    elif partida in ganar:
        print('ganoo')
        cont_puntos += 6

    else: 
        cont_puntos += 0

print(cont_puntos)
```

# Ejercicio entrevista

![Untitled](Hector%20-%20Computer%20Science/Untitled%202.png)

![Untitled](Hector%20-%20Computer%20Science/Untitled%203.png)

![Untitled](Hector%20-%20Computer%20Science/Untitled%204.png)

```python

class PathEngine:
    def __init__(self):
        self.pares = []
        self.x = 0
        self.y = 0
        self.opuestos = {
            'NORTH': 'SOUTH',
            'EAST': 'WEST'
        }

    def _is_repeated_node(self) -> bool:
        return (self.x, self.y) in self.pares
            

    def _add_node_to_visit_list(self):
        self.pares.append((self.x, self.y))

    def is_correct(self, path) -> bool:
        for cardinal in path:
            if cardinal == 'NORTH':
                self.y += 1
                if self._is_repeated_node():
                    return False
                else: self._add_node_to_visit_list()
            elif cardinal == 'SOUTH':
                self.y -= 1
                if self._is_repeated_node():
                    return False
                else: self._add_node_to_visit_list()
            elif cardinal == 'EAST':
                self.x += 1
                if self._is_repeated_node():
                    return False
                else: self._add_node_to_visit_list()
            elif cardinal == 'WEST':
                self.x -= 1
                if self._is_repeated_node():
                    return False
                else: self._add_node_to_visit_list()
        return True

def is_good_path(path):
    engine = PathEngine()
    return engine.is_correct(path)

def test1():
    p1 = ['NORTH', 'NORTH', 'EAST', 'SOUTH']
    assert is_good_path(p1) == True

def test2():
    p1 = ['NORTH', 'WEST', 'SOUTH', 'EAST']
    assert is_good_path(p1) == False

def test3():
    p1 = ['SOUTH', 'EAST', 'SOUTH', 'WEST', 'WEST', 'NORTH', 'EAST']
    assert is_good_path(p1) == False

def test4():
    p1 = ['WEST', 'NORTH', 'EAST', 'SOUTH']
    assert is_good_path(p1) == False

def test5():
    p1 = ['SOUTH', 'WEST', 'NORTH', 'EAST']
    assert is_good_path(p1) == False

def test6():
    p1 = ['SOUTH', 'NORTH']
    assert is_good_path(p1) == False

def test6():
    p1 = ['WEST', 'SOUTH']
    assert is_good_path(p1) == False

def test7():
    p1 = ['NORTH', 'EAST', 'SOUTH','EAST','NORTH','WEST']
    assert is_good_path(p1) == False
```

# Páginas web

[Blockly Games](https://blockly.games/?lang=es)

1. Web 
    1. UI
    2. Backend
    3. Almacenamiento, bases de datos
2. Programación
    1. Lógica, resolver retos
    2. Python para matemáticas, visualización funciones y análisis mat.
3. Análisis de datos
    1. Power BI
    2. Scripting con Python

3. Temario de Computer Science

0