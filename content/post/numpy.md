+++
title = "Matplotlib e Numpy"
date = "2017-08-10T13:09:31+02:00"
tags = []
categories = ["Python"]
menu = ""
+++



```python
# MatplotLib e Numpy
```


```python
## Importando as bibliotecas

import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```


```python
#Crando array com os salarios

salarios = np.array([100,300,200,400])
salarios
```




    array([100, 300, 200, 400])




```python
plt.plot(salarios)
plt.show()
```


![png](/img/numpy/output_3_0.png)



```python
plt.plot(salarios, c = 'Black', ls = '--')
plt.show()
```


![png](/img/numpy/output_4_0.png)



```python
plt.plot(salarios, c = 'Black', ls = '--', marker = 's' )
plt.show()
```


![png](/img/numpy/output_5_0.png)



```python
# Adicionando Label

salario_joao = np.array([100,300,200,400])
salario_rodrigo = np.array([300,250,100,600])
plt.plot(salario_joao, c = 'Black', ls = '--', marker = 's' , label = "Salario João")
plt.plot(salario_rodrigo, c = 'Red', ls = '--', marker = 's' , label = "Salario Rodrigo")
plt.show()
```


![png](/img/numpy/output_6_0.png)



```python
# Adicionando Legenda

plt.plot(salario_joao, c = 'Black', ls = '--', marker = 's' , label = "Salario João")
plt.plot(salario_rodrigo, c = 'Red', ls = '--', marker = '^' , label = "Salario Rodrigo")
plt.legend(loc = 'upper left')
plt.show()
```


![png](/img/numpy/output_7_0.png)

