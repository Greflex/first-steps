# first-steps

"""
def suma(parametro1,parametro2):
    resultado_suma = parametro1 + parametro2
    return resultado_suma

def otrafuncion():
    pi = 3.14
    valor1 = int(input("Numero 1 "))
    valor2 = int(input("Numero 2 "))
    suma_otra_funcion = suma(valor1,valor2) * pi
    return suma_otra_funcion

print(otrafuncion())
"""
"""
n1 = int(input("Ingrese numero uno "))
n2 = int(input("Ingrese numero dos"))
    
if (n1<0 and n2 <0):
    print("Los numeros son negativos ")
elif (n1>0 and n2 >0):
    print("Los numeros son positivos ") 
else:
    print("Son diferentes")
"""
"""
def pnd(n1,n2):
    if (n1 >0 and n2 >0):
        si = "Son positivos"
    elif (n1 <0 and n2 <0):
        si = "Son negativos"
    else:
        si = "Son diferentes"
    return si

n1 = int(input("Ponga numero uno "))
n2 = int(input("Ponga otro "))

print(pnd(n1 ,n2))
"""
"""
def promedio_total(n1,n2,n3):
    promedio = ((n1+n2+n3)/3)
    return promedio 

n1 = int(input("Escriba nota 1 "))
n2 = int(input("Escriba nota 2 "))
n3 = int(input("Escriba nota 3 "))

print("Su promedio total es:",promedio_total(n1,n2,n3))
"""
"""
nota1= float(input("ingrese nota 1: "))
nota2= float(input("ingrese nota 2: "))
nota3= float(input("ingrese nota 3: "))
definitiva=((nota1+nota2+nota3)/3)

def promedio(nota1, nota2, nota3):
  if definitiva > 3.0 :
      p = "bien"
  elif definitiva == 3.0:
      p = "mediocre"
  else:
      p = "mal"
  return p

print("Usted va",promedio(nota1,nota2,nota3),"y su promedio es", definitiva)
"""
"""
edad = int(input("ingresas edad"))
while edad < 18:
    print("aun no soy mayor de edad", edad)
    edad +=1
"""
"""
menu = int(input("ingrese opcion del menu: "))
a = int(input("ingrese numero a operar: "))
b = int(input("ingrese numero a operar: "))
if menu == 1:
    suma = a+b
    print(suma)
elif menu == 2:
    if b > a:
        resta = b - a
    else:
        resta = a - b
    print(resta)
elif menu == 3:
    if a > b:
        division = b / a
    else:
        division = a / b
    print(division)
elif menu == 4:
    multiplicacion = a * b
    print(multiplicacion)
else:
    print("no ingreso numero valido")
"""
"""
edad = 18
sexo = "masculino"
if edad >= 18:
    if sexo == "masculino":
        print("hombre  mayor de edad")
    else:
        print("mujer mayor de edad")
else:
edad = 18
sexo = "masculino"
if edad >= 18:
    if sexo == "masculino":
        print("hombre  mayor de edad")
    else:
        print("mujer mayor de edad")
else:
    print("no soy mayor de edad")
"""
"""
numero = int(input("Ingrese un numero "))
fact = 1
for i in range(1,numero+1):
    fact=fact*i
print(f"El factorial de {numero} es:",fact)
"""
"""
a = 123456789
s = str(a)
for i in s:
    print(i)
"""
"""
total_lista_empleados = 10
empleados = int(input("Empleados: "))
salario_base = 908311
while empleados <= total_lista_empleados:
    comision = salario_base*0.05
    salario = salario_base + comision
    print("nuevo salario", salario, empleados)
    empleados +=1
"""
"""
for i in range (10):
    print (i+1)
"""
"""
for n in range(0,20,5):
    print(n)
"""
"""
numero = int(input("Coloque un numero "))
for i in range(numero):
    if i%2 ==0+1:
        print(i)
"""
"""
def esPrimo(numero):
    for i in range(2,numero):
        if numero % i ==0:
            print("No es primo")
    print("Es primo")

numero = int(input("Coloque un numero "))

for i in range(numero):
    if esPrimo(i):
        print(i)
"""

#Arreglar este codigo------------------------------------------------------------------------------------
"""
num = 10
    for i in range(2,num,1):
        if num % i == 0:
            print("No es primo", i, "es divisor")
    print("Es primo")
        
"""
"""
nume = int(input("Ingrese un numero: "))
if nume % 2 == 0:
    print(f"{nume} es par")
else:
    print(f"{nume} es impar")
"""
"""
num1 = int(input("Ingrese numero 1: "))
num2 = int(input("Ingrese numero 2: "))
num3 = int(input("Ingrese numero 3: "))

if num1 > num2 and num3:
    print("El numero 1 es el mayor")
elif num2 > num1 and num3:
    print("El numero 2 es mayor")
elif num3 > num2 and num1:
    print("El numero 3 es el mayor")
elif num1 == num2 > num3:
    print("El numero 1 y 2 son mayores que el tercero")
elif num1 == num3 > num2:
    print("El numero 1 y 3 son mayores que el segundo")
elif num3 == num2 > num1:
    print("El numero 2 y 3 son mayores que el primero")
else:
    print("Los tres numeros son iguales")
"""
"""
suma = 0
for i in range(300,5001):
    suma = int(suma + i)
print (suma)
"""
#Clases-herencia-poo(Programación orientada a objetos) en Python. SEMANA 3------------------------------------------------------------------------------------
"""
class Galleta:
        def __init__(self, sabor, color):               #inicializamos los atributos de la clase. Este es el constructor
                self.sabor = sabor                      #inicializa atributo sabor. ESte es el atributo xxx...
                self.color = color

sabor = input("ingrese sabor: ")
color = input("ingrese color: ")
galleta = Galleta(sabor, color)                         #Si falta esto, va a dar error

#galleta = Galleta("chocolate", "marron")                #llamamos la clase, no se le debe pasar valores. A la variable le pasamos el objeto

print(f"el sabor de la galleta es {galleta.sabor} y el color es {galleta.color}")


if galleta.sabor == "chocolate":
        print("el sabor de la galleta es de chocolate")
else:
        print("el sabor de la galleta no es chocolate")
"""

class vehiculo():
    def __init__(self,rueda,color,marca):
        self.rueda = rueda
        self.color = color
        self.marca = marca

    def __str__(self):
        return "color{}, ruedas{}, marca{}".format(self.rueda,self.color,self.marca)
        

class Coche(vehiculo):
    def __init__(self,rueda,color,marca,velocidad,motor):
        super().__init__(rueda,color,marca)
        self.velocidad = velocidad
        self.motor = motor
        
#Arreglar esto
    def __str__(self):
        return "velocidad {} km/h, motor {}".format(self.velocidad,self.motor)

coche = Coche("rojo", "4 ruedas", "Chevrolet", "60", "4 tiempos")
print (coche)
#----------------------------------------------------------------------
class Mamiferos:
    def __init__(self, tipo_animal, genero, color, habitat, tipo_alimentacion):
        self.tipo_animal = tipo_animal
        self.genero = genero
        self.color = color
        self.habitat = habitat
        self.tipo_alimentacion = tipo_alimentacion

class Carnivoros(Mamiferos):
    def __init__(self, tipo_animal, genero, color, tamaño):
        self.tipo_animal = tipo_animal
        self.genero = genero
        self.color = color
        self.tamaño = tamaño

carnivoros = Carnivoros("perro", "macho", "cafe", "mediano")
print(f"los atributos de carnivoros es: {carnivoros.tipo_animal}, {carnivoros.genero}, {carnivoros.color}, {carnivoros.tamaño}")
#-----------------------------------------------------------------------------------------------------------------------------
class Terrestre:
    def caminar(self):
        print("el animal camina")
    
    def carnivoro(self):
        print("el animal es carnivoro")


class Acuatico:
    def nadar(self):
        print("el animal nada")


class Pinguino(Terrestre, Acuatico):
    pass

class Perro(Terrestre):
    pass


perro = Perro()
perro.caminar()

pinguino = Pinguino()
pinguino.caminar()
pinguino.nadar()
#-----------------------------------------------------------------------------------------------------------------------------------------------
class Persona:
    def __init__(self):
        self._edad = 0
    # Metodo Getter
    def get_edad(self):
        return self._edad
    
    # Metodo setter
    def set_edad(self, e):
        self._edad = e

edad_maria = int(input("ingrese edad"))
maria = Persona()
maria.set_edad(edad_maria)

print(maria.get_edad())
