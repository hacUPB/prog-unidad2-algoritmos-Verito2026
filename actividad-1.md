# Actividad 1
## Ejercicios
#### 1. ¿Cuántos estados diferentes se pueden representar usando N bits?
Para resolver el ejercicio anterior, intenta con 2 bits, luego con 3 y así sucesivamente. Intenta encontrar una representación matemática para dicha secuencia.   
Representación de estados con bits

2 bits → 4 estados

3 bits → 8 estados

4 bits → 16 estados

N bits → 2ⁿ estados    

---

#### 2. Convierte el número decimal 22 a binario.
Número 22 en binario: 
10110  
  
|16|8|4|2|1|  
|- |-|-|-|-|  
| 1|0|1|1|0|    

---

#### 3. ¿Cuál es el resultado en decimal del número binario 10110?

1(16) + 0(8) + 1(4) + 1(2) + 0(1)= 16 + 4 + 2= 22  
El número 10110 es igual al número 22.  

---

#### 4. ¿Qué número binario representa el carácter 'C' en ASCII?
En ASCII la letra C corresponde al número 67 en decimal, a continuacipon pasaré el 67 a binario.  
|64|32|16|8|4|2|1|  
|- |- |- |-|-|-|-|  
| 1|0|0|0|0|0|1|1|  

---

#### 5. Convierte el número flotante 5.75 a binario (explica los pasos).
Debemos convertir la parte entera y la parte decimal por separado.  
Convertimos 5 a binario  
|4|2|1|  
|-|-|-|  
|1|0|1|

Convertimos la parte decimal  
0.75 x 2 = 1.5 → 1  
0.5  x 2 = 1.0 → 1  
Entonces 0.75 = .11  
Unimos ambas partes    
**Resultado final:** 101.11  

---

#### 6. ¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?  
Debido a que en ASCII cada carácter representa un byte, pues como la palabra "hola" tiene 4 caracteres, entonces se necesitarían 4 bytes para almacenarla.  

---
#### 7.¿Cuántos bits hay en 5 KB?  
Usamos las equivalencias:

- 1 KB = 1024 bytes  
- 1 byte = 8 bits

**Convertimos KB a bytes**

5 × 1024 = **5120 bytes**

**Convertimos bytes a bits**

5120 × 8 = **40960 bits**

**Respuesta:** En **5 KB** hay **40960 bits**.    

---
#### 8. Convierte el número decimal 255 a hexadecimal.  
Si queremos convertir un número decimal a hexadecimal tenemos que dividir el número entre 16.
**Dividimos entre 16**  
 255 / 16 = 15 ; residuo = 15    
 **Conclusiones**  
      -15 en hexadecimal es F  
      -El cociente tambien es 15 ---> F  
**Entonces...**  
255 es igual a FF en hexadecimal.

---
#### 9¿Cuál es el valor hexadecimal de la secuencia binaria 11010110?  
**De derecha a izuiqerda organizamos de 4 en 4 los bits**  
1101   0110  
**Convertir cada grupo usando la tabla**  
      1101 = D  
      0110 = 6  
11010110 (binario) = D6 (hexadecimal)  

---  
## Ejercicios Finales de Repaso

#### 1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.   
Las computadoras representan los datos en binario porque internamente funcionan con electricidad, y los circuitos solo pueden reconocer dos estados: encendido o apagado.
Por eso se usan los valores 0 y 1, ya que son más fáciles de manejar y reducen errores al procesar la información. Todo lo que hace la computadora (texto, imágenes, videos, etc.) se convierte finalmente en combinaciones de esos dos valores.  
 
#### 2. Convierte el número binario 10011011 a decimal y a hexadecimal.    

|128|64|32|16|8|4|2|1|  
|---|- |- |- |-|-|-|-|  
| 1 |0 |0 |1 |1|0|1|1| 

128+ 16 + 8 + 2 + 1 = 155|   

Para pasarlo a hexadecimal, agrupo de 4 en 4:

1001 1011

1001 = 9

1011 = B


#### 3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.  
Una imagen PNG se guarda como un archivo formado por datos binarios. Dentro del archivo se almacena información como el tamaño de la imagen, los colores y la posición de cada píxel.
Cada píxel se representa con números que indican sus colores (rojo, verde y azul, y a veces transparencia). Además, el formato PNG comprime la información para que el archivo pese menos sin perder calidad.  
#### 4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?

Un byte solo puede almacenar valores entre 0 y 255. Como 300 es mayor que ese límite, no cabe en un solo byte.

En Python, los números enteros no tienen un límite fijo como en otros lenguajes, porque el programa usa automáticamente más memoria cuando el número es grande. Por eso Python sí puede manejar el número 300 sin problema, usando más de un byte internamente.