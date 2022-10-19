# 10219106
Shafira Amaliyah


## materi sebelumnya
+ Persamaan diferensial
+ Predator-prey
+ Lorentz attractor
+ Rekursif faktorial
+ Runge-Kutta orde 4
+ Metode euler
+ Osilasi harmonik sederhana
+ Monte Carlo 
+ Matriks difusi panas 
+ DFT & FFT/ Transformasi Euler


## materi paling menarik
+ Monte Carlo 
+ 2D heat equation

## materi paling membosankan
+ Osilasi harmonik sederhana 

## materi yang sudah dipahami
+ Metode numerik (Runge-Kutta dan Euler) untuk Kasus Predator-Prey
+ 2D heat equation
+ Monte carlo 
+ dll

## materi yang belum dipahami
+ DFT dan FFT

## contoh program

```python
# contoh program python: Monte Carlo (Memanfaatkan bilangan acak untuk menentukan bilangan pi)
import matplotlib.pyplot as plt
import random

inside = 0
n = 10000

x_inside = []
y_inside = []
x_outside = []
y_outside = []

for _ in range(n):
    x = random.uniform(-1,1)
    y = random.uniform(-1,1)
    if x**2 + y**2 <= 1 :
        inside += 1
        x_inside.append(x)
        y_inside.append(y)
    else:
        x_outside.append(x)
        y_outside.append(y)      
        
pi = 4*inside/n
print(pi)

fig, ax = plt.subplots()
ax.set_aspect('equal')
ax.scatter(x_inside, y_inside, color='g', marker='s')
ax.scatter(x_outside, y_outside, color='r', marker='s')

plt.draw()

```

Hasilnya adalah 3.1652

![image](https://user-images.githubusercontent.com/95624771/196589422-ea18afb5-4719-4fda-b256-bddd6d28e116.png)


```

```


## cara perkuliahan
+ Usulan saya: akan lebih baik apabila dosen mempersiapkan PPT untuk materi agar waktu di kelas tidak dihabiskan untuk menulis di papan tulis. 
+ Selain itu, saya mengusulkan untuk kuliah online pada beberapa pertemuan


## topik sistem fisis
+ Sistem fisis yang menarik bagi saya untuk dikaji lebih dalam adalah terkait finite element method di sistem fisis kompleks


## simulasi dan visualisasi
+ Saya tertarik sengan simulasi dan visualisasi, topik yang ingin saya simulasikan adalah terkait multilateration
+ Perkiraan pustaka Python yang perlu digunakan adalah: https://github.com/glucee/Multilateration, https://pypi.org/project/Localization/
