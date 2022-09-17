## Clase 16 de Agosto: Ejercicio 1: Imprimir mensaje, ver id (espacio de memoria donde se almacena una variable)
```python
print("Hola Mundo")
x=10
print(x,":",id(x))
```
## Clase 22 de Agosto: Ejercicio 2: Uso y declaración de funciones 
```python
def mensaje(msg):
    print(x)

x = "Hola Mundo"

mensaje(x)
x="Hola mundo"
x:int=10

print(x)

print(x)

# %% (ejecutar bloque de código)
print ("Hola ICI")
x=10

# %% (ejecutar bloque de código)
print ("Hola")
print (x)

# %% (ejecutar bloque de código)
x=10
print(x,":",id(x))

x=x+1
print(x,":",id(x))

# %% (ejecutar bloque de código)
def mensaje(msg:str):
    print("Dentro de la funcion",msg,id(msg))

x = "Hola Mundo"
print("Fuera de la funcion",x,id(x))
mensaje(x)
# %% (ejecutar bloque de código)
if __name__=="__main__":
    mensaje("Hola Mundo")

def saludo_edad_(nombre:str,a_nacimiento:int):
    edad= 2022-a_nacimiento
    print("Hola",nombre,"tienes",edad,"años")
if __name__=="__main__":
    saludo_edad_("Olga",2003)
```
## Clase del 29 de Agosto: Ejercico 3: Uso de libretas en Jupyther
```python
## Uso de markdown en Jupyther y código 
# Universidad de Colima
# Facultad de ingeniería Mecánica y Eléctrica
# Ingeniería en computación Inteligente
print ("Hola")
#Interpolación de cadenas 
name="Alex"
edad=18
print("Hola",name,"tienes",edad,"años")
#fString 
mensaje=f"Hola {name}, tienes {edad} años"
mensaje
print(mensaje)
print(f"Hola {name}, tienes {edad} años")
def saludo():
    print("Hola mundo!!!")
mi_funcion= saludo() #Asignando la funcion
saludo() #invocando la funcion 
print(mi_funcion)
def saludo2():
    return "HOLA MUNDO!!!"
saludo2() #invocacion 
mi_funcion2=saludo2 #asignarla 
print(mi_funcion2)
a=5
b=10
res=f" La suma de {a} + {b} = {a+b}"
print (res)
def suma (a,b):
    return a+b
res=f"La suma de  {a} + {b} = {suma (a,b)}"
print (res)
lista_numeros=["uno","dos","tres"]
msg_numeros=f"numeros:{lista}"
print(msg_numeros)
tupla_numeros=("uno","dos","tres",)
msg_numeros=f"Numeros: {tupla_numeros}"
print (msg_numeros)
set_numeros={"uno","dos","tres","tres"}
print(set_numeros)
dict_numeros={"1":"uno","2":"dos","3":"tres"}
msg_dict_numeros=f"Numeros: {dict_numeros}"
print(msg_dict_numeros)
msg_dict_numeros=f"Numero: {dict_numeros['2']}"
print (msg_dict_numeros)
def msj (nombre:str,ac:int,anac:int)-> str:
    return f"Hola {nombre} tines {ac-anac} años"
print (msj("Olga",2022,2003))
num_materia=["No.",1,2,3,4]
name_materia=["Materia","Estructura de Datos","Ecuaciones Diferenciales","Metodos Numericos","Programacion Funcional"]
name_profesor=["Profesor","Soto","Eli","Edgar","Walter"]
print (f"{num_materia[0]:^5}{name_materia[0]:^30}{name_profesor[0]:<6}")
for i in range (1,5):
    print (f"{num_materia[i]:^5}{name_materia[i]:<30}{name_profesor[i]:<6}")
```
## Clase 30 de Agosto: Ejercicio 4: Uso de f'Strings
```python
name_alu=["Hugo","Paco","Luis","Paola","Laura"]
name_materia1=[10,9,10,8,10]
name_materia2=[7,7,8,7,9]
name_materia3=[6,7,8,9,5]
name_materia4=[6,6,7,6,7]

encabezado=["Nombre","Est. de Datos","Ec. Diferenciales","Met. Numericos","Prog. Funcional"]

def reporte(fmt):
    print (f"{encabezado[0]:^{fmt}} {encabezado[1]:^{fmt}} {encabezado[2]:^{fmt}} {encabezado[3]:^{fmt}} {encabezado[4]:^{fmt}}")
    for i in range (5):
        print (f"{name_alu[i]:^{fmt}} {name_materia1[i]:^{fmt}} {name_materia2[i]:^{fmt}} {name_materia3[i]:^{fmt}} {name_materia4[i]:^{fmt}}")
reporte(20)

def reporte(fmt):
    print (f"{encabezado[0]:^{fmt}} {encabezado[1]:^{fmt}} {encabezado[2]:^{fmt}} {encabezado[3]:^{fmt}} {encabezado[4]:^{fmt}}")
    for i in range (5):
        print (f"{name_alu[i]:*^{fmt}} {name_materia1[i]:*^{fmt}} {name_materia2[i]:*^{fmt}} {name_materia3[i]:*^{fmt}} {name_materia4[i]:*^{fmt}}")
reporte(20)

fmt=20
print (f"{name_alu[0]:+^{fmt}}")

print (f"{name_alu[0]:+>{fmt}}")
print (f"{name_alu[0]:+<{fmt}}")
numero_big=1000000000076766
print(f"{numero_big:,d}")
print (10/3)
num=10/3
print (num)
print (f"{num:.2f}")
print(f"{num:e}")
num=33124.47468373
print(f"{num:e}")
porcentaje= 0.257864273892
print (f"{porcentaje:%}")
print(f"{porcentaje:.3%}")
print (f"{255:o}")
print (f"{255:x}")
print (f"{255:b}")
print (f"{65:c}")
for i in range (255):
    print (f"{i:^10}:{i:c}")
## Clase 05 de Septiembre: Ejercicio 5: Importar archivos para uso de funciones en otro
```python
def resta(num: int, num2: int) -> int: return num - num2


if __name__ == "__main__":
    print(resta(3, 7))
import re
from threading import currentThread


mi_lista=[1,2,3,4]
print(mi_lista)
lista_vacia=[]
print(lista_vacia)
 

mi_lista2=[1,"Hola",True,3.14,[1,2,3],(1,2,3),{1,2,3}]
print(mi_lista2)

print(len(mi_lista))
print(len(mi_lista2))
print(f"Mi lista:{mi_lista}")

print(f"No de elementos:{len (mi_lista)}")
print(f"Primer elemento:{mi_lista[0]},{mi_lista[1]},{mi_lista[2]},{mi_lista[3]}")
print(f"Primer elemento:{mi_lista[-1]},{mi_lista[-2]},{mi_lista[-3]},{mi_lista[-4]}")

#Slices: rebanadas (partes de una lista)
print(mi_lista[1:-1])
print(mi_lista[0:3])
print(mi_lista[0:])
print(mi_lista[:])

#modificar elementos de la lista

mi_lista[2]="tres"
print(mi_lista)

#Insertar la lista [5,"seis",7,8] al final de la lista mi_lista 
new_lista=[5,"seis",7,8]
mi_lista[len(mi_lista):]=new_lista
print(mi_lista)

mi_lista=[1,2,3,4]
mi_lista.append("cinco")
print(mi_lista)

ml=[]
for i in range(1,5):
    ml.append(i)
print(ml)

#ml.append([6,7,8])
#print(ml)
ml.extend([6,7,8])
print(ml)

ml.insert(4,"cinco")
print(ml)

del ml[5]
print(ml)

ml.remove(2)
print(ml)

ml.reverse()
print(ml)

l1=[1,2,3]
l2=l1[:]
print(l1)
l1.reverse()
print(l1)
print(l2)
```
## Clase 6 de Septiembre: Ejercicio 6: Uso de las listas: 
```python
ld=[[5,4,6],[7,8,2,1],[3,4,5],[6,7]]
print(f"Desordenado: {ld}")
ld.sort()
print(f"Ordenado: {ld}")

ld=[5,4,6,7,8,2,1,3,4,5,6,7]
S1= sorted(ld)
print(S1)
ld=[5,4,6,7,8,2,1,3,4,5,6,7]
S2= sorted(ld,reverse=True)
print(S2)

ceros=[0,0,0,0,0,0,0,0,0]
print(ceros)
ceros=[0]*9
print(ceros)

valor_max=max(ld)
print(valor_max)

valor_min=min(ld)
print(valor_min)

cuatros=ld.count(4)
print(cuatros)

repe=[]
for i in range (1,9):
    repe.append(ld.count(i))
print(repe)

#Escribe una funcion que reciba como argumentos T y N donde T
#  es el limite de tablas de multiplicar  que se desean obtener
# y N hasta un valor de las tablas se desea. Todas empiezan desde 1

def tablas(t:int,n:int):
    for i in range(1,t+1):
        tabla(i,n,10)

def tabla(t:int,n:int,spc:int):
    for i in range (1,n+1):
        print(f"{t:^{spc}}x{i:^{spc}}={t*i:^{spc}}")

t=int(input("¿Hasta que tablas quieres calcular?"))
n= int(input("¿Hasta que numero quieres calcular?"))
tablas(t,n)
```
## Clase 12 de Septiembre: Ejercicio 7: Uso de funciones con ciclo for y f'strings
```python
def tabla(t,n):
    for i in range (1,n+1):
        print(t,"*",i,"=",t*i)
if __name__=="__main__":
    print(tabla(3,2))
# %% (ejecutar bloque de código)
def tabla(t:int,n:int,spc:int):
    for i in range (1,t+1):
        for j in range (1,n+1):
            print(f""i,"*",j,"=",i*j)
t=int(input("¿Hasta que tablas quieres calcular?"))
n=int(input("¿Hasta que numero quieres calcular?"))
tabla(t,n)
# %% (ejecutar bloque de código)
def tabla(t:int,n:int,spc:int):
    for i in range (1,t+1):
        for j in range (1,n+1):
            print(f"{i:^{spc}} * {j:^{spc}} = {i*j:^{spc}}")
t=int(input("¿Hasta que tablas quieres calcular?"))
n=int(input("¿Hasta que numero quieres calcular?"))
spc=int(input("¿Que espaciado quieres?"))
tabla(t,n,spc)
```
