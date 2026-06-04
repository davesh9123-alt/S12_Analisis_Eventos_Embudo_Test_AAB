# Analisis basado en eventos y test A/A/B

En este proyecto analizamos el embudo de ventas de una tienda online de productos alimenticios. Investigamos el comportamiento de los usuarios de la app de la empresa. Posteriormente analizamos los resultados de la prueba A/A/B que realizaron. La prueba consistio en cambios en el tipo de fuente para las letras de la aplicacion. Es decir, dos grupos (grupos A) se les dio la version antigua con fuentes originales y el grupo experimental (grupo B) se le dio una version con fuentes nuevas. Nuestra tarea consistio en descubrir que version tiene mejores resultados.

**Objetivos**: Descubrir que version de la aplicacion tiene mejores resultado para las ventas. Se busca al menos un 10% de mejora en las ventas con la nueva version.


## Habilidades Tecnológicas Utilizadas

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75.svg?style=for-the-badge&logo=Plotly&logoColor=white)
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![Postgresql](https://img.shields.io/badge/PostgreSQL-4169E1.svg?style=for-the-badge&logo=PostgreSQL&logoColor=white)
![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-%2334A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)


## Preguntas clave

- ¿Que proporcion de usuarios pasan de una etapa a la siguiente?
- ¿En que etapa se pierden mas usuarios?
- ¿Que porcentaje de usuarios hace todo el viaje desde el primer evento hasta el pago?


## ¿Que proporcion de usuarios pasan de una etapa a la siguiente? - Enbudo de Eventos

De acuerdo a los resultados del embudo de eventos, la etapa en la que se pierden mas usuarios es de Main Screen a Offers Screen. Solo 61.9% de la etapa anterior continuan hacia la pagina de Offers. Cerca de un 40% de usuarios no pasan de la Main Screen a la etapa siguiente.

* MainScreenAppear: 7419 usuarios --> 100%
* OffersScreenAppear: 4593 usuarios --> 61.9% --> 61.9% de la cantidad de arriba
* CartScreenAppear: 3734 usuarios --> 50.3% --> 81.3 de la cantidad de arriba
* PaymentScreenSuccessful: 3539 usuarios --> 47.7% --> 94.8% de la cantidad de arriba
* Tutorial: 840 usuarios --> 11.3% --> 23.7% de la cantidad anterior

<img width="1223" height="362" alt="Screenshot_20260604164037" src="https://github.com/user-attachments/assets/437ecf68-16d3-42b2-9319-56bbad32abd9" />


## Resultados de las pruebas de Hipotesis para el test A/A/B

Realizamos las pruebas con dos diferentes valores de significancia alpha, 0.05 y 0.01. En ambos, los resultados fueron similares. Parece que modificar las fuentes no ha tenido ningun efecto en el comportamiento de los usuarios al usar la app. Los resultados de los grupos de control y el grupo experimental se muestran muy similares y segun la prueba realizada podemos concluir que no ha causado ninguna diferencia el modificar las fuentes de la app.

<img width="707" height="574" alt="Screenshot_20260604164409" src="https://github.com/user-attachments/assets/eb349339-a061-4d4f-93bd-f9e40b77bdf2" />


## Conclusiones

Los resultados parecen ser bastante concluyentes. Aun combinando ambos grupos de control contra el grupo experimental, el resultado de la prueba nos dice que no hay diferencia significativa entre los grupos. Esto quiere decir que el grupo experimental no ha dado resultados negativos pero tampoco positivos. Simplemente, los cambios en las fuentes de la app no han provocado cambio alguno pues el comportamiento de los usuarios es practicamente igual.

El objetivo no fue logrado, no existe una diferencia significativa en los grupos.
