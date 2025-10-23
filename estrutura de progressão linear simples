#Importando as Bibliotecas:

import numpy as np #Cálculos científicos em Python.
import pandas as pd #Utilizada para manusear bancos de dados.
import matplotlib.pyplot as plt #Plotagem de gráficos.
from sklearn.linear_model import LinearRegression #Scikit Learn: Machine Learning em Python.

#Carregando a base:

base = pd.read_excel ("")

base.head (10)

x = base [["anos"]]
y = base ["salários"]

#Treinando o Modelo:

modelo = LinearRegression ()

modelo.fit (x, y)

#Coeficientes:

#Intercepto (a): Ponto que cruza o eixo vertical (y).
#Inclinação/Coeficiente (b): Quanto que y altera de acordo com x.

print (f"Intercepto (a): {modelo.intercept_:.2f}")
print (f'Inclinação (b): {modelo.coef_[0]:.2f}')

#Prever o salário para o ano X de colaboração na empresa:

salario = modelo.predict ([[]])

print (f'Salário: R$ {salario[0]:.2f}')

#Gráfico de Dispersão:

plt.scatter (x, y, color = 'blue', label = 'Dados reais')
plt.scatter (8, salario, color ='green', label = 'Salario previsto')
plt.plot (x, modelo.predict (x), color ='red', label ='Reta/Regressão')
plt.title ("Regressão Linear")
plt.xlabel ('Anos de Empresa')
plt.ylabel ('Salários R$')
plt.legend ()
plt.grid ()
plt.show ()
