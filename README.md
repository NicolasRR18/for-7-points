# for-7-points
# WHILE-RETO-6

=============================================================

El objetivo era resolver el reto 6, el cual consistia en
realizar algoritmos que cumplieran con las necesidades 
planteadas en cada punto, y para los primeros 3 puntos
adjuntar un .
A continuacion adjunto la imagen del repo del profe Felipe:

============================================================

![image](https://github.com/user-attachments/assets/470b6871-8708-468d-ba0e-bd5a697e7465)

============================================================

 >-Asi que adjuntare capturas mostrando como estan
 >diseñados los codigos para cumplir con cada punto del reto,
 >los realice en visual studio code, a su vez adjuntaré
 >los codigos para que puedan ser copiados y probados.

============================================================

![image](https://github.com/user-attachments/assets/289d2f14-149c-49ba-b868-4c24e935a27f)

```

def cuadrados_2(n:int) -> int:
    return n ** 2
for n in range(1, 100 + 1, 1):
    cuadrado_2 = cuadrados_2(n)
    print(cuadrado_2)

```

============================================================

![image](https://github.com/user-attachments/assets/163a0ede-462e-45ef-8eb0-164bce7fa6d4)

```

n = 0
x = 1
print ("Listado de numeros impares hasta el 999: ")
for n in range (0, 1000, (2 * n) + 1 ):
    if (2 * n) + 1 <= 1000:
        print((2 * n) + 1)
print ("y hasta aquí el listado de los impares")

print ("Listado de numeros pares hasta el 1000: ")
for x in range (1, 1000):
    if (2 * x) <= 1000:
        print ((2 * x))
print ("y hasta aquí el listado de los pares")

```

============================================================

![image](https://github.com/user-attachments/assets/53851f7a-ed46-489b-9b42-ab05f929dedd)

```

n = int(input("digite un numero cualquiera mayor a 2 :"))
for n in range (n, 1, -1):
    if n % 2 == 0 and n >= 2:
        print(n)

```

============================================================

![image](https://github.com/user-attachments/assets/4c24e21f-671b-4dfe-a335-6cc1f7b3b836)

```

n = int(input("Ingrese un numero cualquiera mayor a 0"))
multiplicacion: int = 1
for i in range (1, n+1):
    multiplicacion *= i
    print("El factorial de", (i), "es", multiplicacion)

```

============================================================

![image](https://github.com/user-attachments/assets/c12a9163-7f1e-4b86-8686-ed5784ee41ca)

```

n = int(input("Ingrese una potencia entera positiva para 2"))
if n > 1:
    x = 2
    for i in range (2, n+1):
        x *= 2
    print(x)
elif n == 1:
    print (2)
elif n == 0:
    print (1)

```

============================================================

![image](https://github.com/user-attachments/assets/030d86f7-93f3-499e-8694-1ad184e342cc)

```

n = int(input("Ingrese un numero natural:"))
x = float(input("Ingrese un numero natural:"))
elevado = 1.0
for i in range (n):
    elevado *= x
print(elevado)
#elif x == 0:
   # print (1)

```

============================================================

![image](https://github.com/user-attachments/assets/9407f69d-0185-4c8b-85d0-99659321356c)

```

for i in range (1, 10):
    for n in range (1, 11):
        i * n
        print((i), "x",(n), "=",( i * n ))

```

============================================================

![image](https://github.com/user-attachments/assets/41ad811d-4185-4fa3-b13f-c3de513e8187)

```

import math

def sin_maclaurin(x, n):
 
    result = 0
    
    # Sumatoria de los términos de la serie de Maclaurin
    for i in range(n):
        # Calculamos (-1)^i * x^(2i+1) / (2i+1)!
        numerator = (-1) ** i * (x ** (2*i + 1))
        denominator = math.factorial(2*i + 1)
        term = numerator / denominator
        result += term
    
    return result

def compare_sin(x, n):
    real_value = math.sin(x)
    approximation = sin_maclaurin(x, n)
    error = abs(real_value - approximation)
    
    return real_value, approximation, error

# Ejemplo de uso
x = math.pi/4  # 45 grados
terms = 5
real, approx, error = compare_sin(x, terms)

print(f"x = {x} radianes ({math.degrees(x):.2f} grados)")
print(f"Términos utilizados: {terms}")
print(f"Valor real de sin({x:.4f}): {real:.10f}")
print(f"Aproximación: {approx:.10f}")
print(f"Error absoluto: {error:.10f}")

```

============================================================

![image](https://github.com/user-attachments/assets/7b65ea6e-9683-4a9a-8270-37981d50ca09)

```

import math

def exp_taylor(x, n):

    result = 0
    
    # Sumatoria de los términos de la serie de Taylor
    for i in range(n):
        # Calculamos x^i / i!
        term = (x ** i) / math.factorial(i)
        result += term
    
    return result

def compare_exp(x, n):

    real_value = math.exp(x)
    approximation = exp_taylor(x, n)
    error = abs(real_value - approximation)
    
    return real_value, approximation, error

# Ejemplo de uso
x = 2
terms = 10
real, approx, error = compare_exp(x, terms)

print(f"x = {x}")
print(f"Términos utilizados: {terms}")
print(f"Valor real de e^{x}: {real:.10f}")
print(f"Aproximación: {approx:.10f}")
print(f"Error absoluto: {error:.10f}")

```

============================================================

# NICOLAS RAMIREZ RODRIGUEZ 1000506513
