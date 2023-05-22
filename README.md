# CRO

<p align="center">
  <img src="https://github.com/Anton-Utray/CRO/blob/main/IMG/Portada-CRO.jpg" alt="Portada" width="500">
</p>


1. [Objetivo](#objetivo)
2. [Descripción](#descripcion-del-proyecto)
3. [Prototipo](#prototipo)
4. [Analisis y Conclusiones](#analisis)


## Objetivo

Proyecto colaborativo con el bootcamp UX/UI donde el objetivo es optimizar la tasa de conversión de un ecommerce a través de una versión control (original) y una de testeo (con cambios) para analizar y comparar el rendimento entre ambas versiones. 

Flujo de trabajo:

 - UX/UI presenta el prototipo de su pagina web al equipo de data. En nuestro caso se trata de una pagina web de venta de libros Altamerea. 
 - Data salimos a recopilar datos de uso, preguntando a voluntarios de probar el prototipo. 
    - Se pregunta a los voluntarios: 
        - Buscar los libros de la categoria femenina
        - Dentro de la categoria femenina encontrar los que corresponden a tapa dura
        - Encontrar el libro de Michelle Obama y completar el checkout. 
    - Nos encargamos de medir: el tiempo en realizar diversas acciones.
    - Clicks totales vs clicks utiles.
    - Comentarios de tipo general que nos den **feedback** general.
- Reunion entre ambos equipos para retroalimentar y decidir sobre los cambios a efectuar para la versión control. 
- Segunda recopilación de datos de campo. 
- Alimentación de datos al sistema para medir y cuantificar las mejoras. 

**KPIS** 

El objetivo es optimizar la tasa de clicks utiles vs clicks totales en el proceso de compra. De igual manera tenemos como objetivo reducir la media de tiempo para finalizar la compra. 

Para tal efecto, definimos los siguientes KPIs como objetivo:

 - Tasa de clicks para realizar compra: 12
 - Tiempo para realizar checkout: 1 minuto. 

 Estos KPIS luego nos van a servir a la hora de categorizar los resultados (True/False) para efectuar un modelo bayesiano. 

## Prototipo

<p align="center">
  <img src="https://github.com/Anton-Utray/CRO/blob/main/IMG/cambios%20web.png" alt="Cambios" width="800">
</p>


Los cambios fueron: filtro desplegable para que el usuario visualice directamente las opciones, opción de pagar ya directamente en el thumbnail de los productos en el landing. Antes tenian que entrar dentro del product page antes de que apareciese la opción. De igual manera el esquema de color entre el botón de cesta era color rojo y el pagar ya estaba con fondo blanco y letras en negro. Por lo tanto el cliente iba directo a agregar a cesta en vez del checkout, agregando un click adicional

## Analisis y Conclusiones

Por un lado hemos trabajado con el minimo de clicks que puede realizar un usuario en todo el proceso de una compra.

- En la primera pagina el minimo es de 13, pero por ciertos metodos de construccion tendia a 18 y el tiempo promedio era de 1:30 min
- En la segunda pagina el minimo es de 10, y este en la reconstruccion tiende hasta 14 y el tiempo promedio es de 50 seg 

</div>
<div align="center">
  Aqui el grafico de como queda al final para cada uno:
  
  ![image](https://github.com/joeSL-ms/proye/assets/127346073/590e48b6-dd3b-41df-91ee-e3502f26c00b)
  
  Aqui el grafico de las medias para cada estudio:
  
  ![image](https://github.com/joeSL-ms/proye/assets/127346073/cded53a4-8422-4531-aa3e-045fce8bffe9)
</div>
<div>
  Como podemos observar a ojo hay una cierta diferencia, pero vamos a llevarlo mas lejos y confirma cuanta probabilidad hay para cada caso.

| Clicks | Tiempo |
| --------- | --------- |
| Caso 1 | Caso 2 |
|  En vase a la tasa de click hemos obtenido que la tasa de conversion en un 400.00%, con una probabilidad del 99.90%. Dando una seguirad de mejoria   | Usando la informacion del tiempo sabemos que la tasa de conversion en un 116.67%, con una probabilidad del 99.43%.   |
| <div align="center" colspan="2"> ![image](https://github.com/joeSL-ms/proye/assets/127346073/af1933f5-c203-4873-a0b0-5c83badce8a2)</div> | <div align="center"> ![image](https://github.com/joeSL-ms/proye/assets/127346073/284b07c1-bbac-47ee-854a-09749ab21411)</div> |
  </div>
