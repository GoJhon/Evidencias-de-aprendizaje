# Evidencias-de-aprendizaje
Anotaciones de actividades en ADSO Sena

## Hoja de vida

Utilizamos el lenguaje marcado Markdown para crear una hoja de vida en Github.

[Hoja de vida](https://github.com/GoJhon/Hoja-de-vida.git)

![Hoja de vida](https://i.imgur.com/mqTt1jV.png)

## Visual Basic

Aprendimos que antes de programar se tienen crear un **algoritmo** y un **diagrama de flujo**. También a crear variables y pops en Visual Basic.

**Algoritmo**

![Algoritmo](https://i.imgur.com/ngAbeE5.jpg)

**Diagrama de flujo**

![Diagrama de flujo](https://i.imgur.com/xubGtkq.png)

**Visual Basic**

```
    Sub introduccion()
    nom = "Luis"
    MsgBox (nom)
    num = 10
    MsgBox (num)
    nom = "Maria"
    MsgBox ("El nombre es: " & nom)
    End Sub
```

## Kanban, asignación de variables y contenación

Aprendimos sobre kanban un metodo de orgazación de datos. Realizamos un desafio sobre crear un promedio entre 3 variables

**Desafío**

![Desafio promedio de 3 variables](https://i.imgur.com/k8tAGFn.jpg)

**Kanban**

![Kanban](https://i.imgur.com/P24lp7u.jpg)

## Github desktop y condicionales

Aprendimos a manejar un software llamada "Github desktop" que sirve para clonar repositorios y subirlos a la plataforma github. Realizamos un desafio sobre crear una condición entre el 5% y 10%

**Github Desktop**

![Github Desktop](https://i.imgur.com/4hXPf6z.png)

**Desafío descuentre del 5% y 10%**

**Algoritmo**

![Algoritmo descuento](https://i.imgur.com/XWvmaEa.jpg)

**Diagrama de flujo**

![Diagrama de flujo descuento](https://i.imgur.com/zP5sSl9.jpg)

**Codigo en Visual Basic**

```
Sub Descuentos()
    cantidadObjetos = Int(InputBox("La cantidad de objetos son: "))
    precioTotal = Int(InputBox("El precio total es:"))
    If cantidadObjetos > 10 And cantidadObjetos <= 20 Then
        descontarCinco = (precioTotal * 5) / 100
        descuentoCinco = precioTotal - descontarCinco
        MsgBox ("El precio a pagar es: " & descuentoCinco)
    Else
        If cantidadObjetos > 20 Then
            descontarDiez = (precioTotal * 10) / 100
            descuentoDiez = precioTotal - descontarDiez
            MsgBox ("El precio a pagar es: " & descuentoDiez)
        Else
            MsgBox ("El precio es: " & precioTotal)
        End If
    End If
End Sub
```

## Desafío grupal

Hubo un desafío grupol que trabajo de crear una logica de condiciones y asginar variables.

**Algotimo**

![Algoritmo grupal](https://i.imgur.com/fkZOzxI.jpg)

**Diagrama de Flujo**

![Diagrama grupal](https://i.imgur.com/EHIoKra.jpg)
