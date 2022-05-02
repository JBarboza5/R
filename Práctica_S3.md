---
title: "Lenguaje de Programación R"
author: "Jemina Barboza"
date: "2022/05/01"
output:
  html_document:
    code_download: TRUE
    toc: true
    toc_float: true
---

### **¿QUÉ ES R?**

R es un entorno y lenguaje de programación libre que se utiliza para el procesamiento y análisis estadístico.

> Es importante mencionar que R es el lenguaje de programación utilizado para el análisis de datos, a diferencia de R Studio que es el entorno de desarrollo integrado (IDE).

<center>

![](imagen.jpg){width="190"}

</center>

### **CARACTERÍSTICAS**

-   Enorme potencial para el análisis de datos

-   Es software libre disponible para todos los sistemas operativos (Windows, Mac OS, Linux).

-   Ambiente de trabajo muy flexible y extensible

-   Tiene la posibilidad de cargar diferentes bibliotecas/paquetes aumentando sus posibilidades

-   Trabaja con otros lenguajes y permite leer datos de otros softwares como SPSS, SAS, Excel, etc.

-   Puedes crear aplicaciones web interactivas (apps) con la herramienta Shiny.

-   Puedes crear un flujos de trabajo para escribir informes reproductibles y dinámicos y hacerlo en varios formatos (PDF, Word, html).

### **¿CÓMO INSTALAR R?**

<center>

<iframe width="560" height="315" src="https://www.youtube.com/embed/k0oCZdJPsDU" frameborder="0" allowfullscreen data-external="1">

</iframe>

</iframe>

</center>

### **APLICACIONES DE R**

1.  ***Realizar operaciones matemáticas***

+:---------------:+:------------------------:+:---------------:+:-------------:+
| **Operador**    | **Operación**            | **Ejemplo**     | **Resultado** |
+-----------------+--------------------------+-----------------+---------------+
| exp(n)          | Eleva e a la n           | exp(3)          | 20.085        |
+-----------------+--------------------------+-----------------+---------------+
| sqrt(n)         | Raíz cuadrada de n       | sqrt(3)         | 1.732         |
+-----------------+--------------------------+-----------------+---------------+
| log(n)          | Logaritmo natural de n   | log(3)          | 1.098         |
+-----------------+--------------------------+-----------------+---------------+
| log(n, b)       | Logaritmo de n en base b | log(3, 10)      | 0.477         |
+-----------------+--------------------------+-----------------+---------------+
| log2(n)         | Logaritmo en base 2      | log2()          | 3.322         |
+-----------------+--------------------------+-----------------+---------------+
| pi              | Número pi                | Pi              | 3.146         |
+-----------------+--------------------------+-----------------+---------------+
| abs(n)          | Convierte n en absoluto  | abs(-10.2)      | 10.2          |
+-----------------+--------------------------+-----------------+---------------+

2.  ***Realizar gráficos de barras***

Para ello, debemos seguir los siguientes pasos:

    x <- table(mtcars$cyl)
    colores <- c("orange","skyblue","yellow3")

    library(ggplot2)

    ggplot(mtcars,aes(cyl)) + geom_bar(fill=colores) + labs(x="Cilindros", y="Frecuencia", title="Número de Cilindros") + theme_gray()

<center>

![](Nro%20de%20Clindros.png){width="792"}

</center>

3.  ***Utilizar sintaxis y comandos LaTeX***

```{=html}
<!-- -->
```
a.   Fórmulas Matemáticas

$$
a^2 + b^2 = c^2
$$


$$
\text{Ecuación 2do Grado} \quad x=\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

b.  Fórmulas químicas

$$
Cl_2 + 2Na  ->  2NaCl
$$


$$
6H_2O + 6CO_2  ->  C_6H_12O_6 + 6O_2
$$

<div class="tocify-extend-page" data-unique-"tocify-extend-page" style-height: :"></div>
