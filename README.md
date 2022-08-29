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

## Desafío del hotel y noches

Se creo un desafio en donde si habian más de 3 noches hospedadas se le hacia un descuento del 5%

**Algoritmo**

![Algoritmo hotel](https://i.imgur.com/RwzMBSL.jpg)

**Diagrama de flujo**

![Diagrama hotel](https://i.imgur.com/I4Mf5O2.jpg)

**Visual Basic**

```
Sub Hotel()
    nombreCliente = InputBox("nombre del cliente")
    totalNoches = Int(InputBox("noches a hospedar"))
    precioNoches = totalNoches * 100
    If totalNoches <= 3 Then
        MsgBox (nombreCliente & " se va hospedar " & totalNoches & " noche(s) y debe pagar: " & precioNoches)
    Else
        descontar = (precioNoches * 5) / 100
        descuento = precioNoches - descontar
        MsgBox (nombreCliente & " se va hospedar " & totalNoches & " y debe pagar " & descuento)
    End If
End Sub
```

## Sacar impuesto según los ingreso anuales de una empresa

**Con condición if**

```
Sub genradorImpuesto()
    MsgBox ("Bienvenidos a la IDAN")
    ingresos = Int(InputBox("Digite sus ingresos anuales"))
    If ingresos >= 0 And ingresos <= 1000 Then
        MsgBox ("No debe pagar impuestos")
    Else
        If ingresos >= 1001 And ingresos <= 10000 Then
            impuesto = (ingresos * 5) / 100
            MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
        Else
            If ingresos >= 10001 And ingresos <= 100000 Then
                impuesto = (ingresos * 10) / 100
                MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
            Else
                If ingresos >= 100001 And ingresos <= 1000000 Then
                    impuesto = (ingresos * 15) / 100
                    MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
                Else
                    If ingresos >= 1000001 And ingresos <= 10000000 Then
                        impuesto = (ingresos * 20) / 100
                        MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
                    Else
                        If ingresos >= 10000001 Then
                            impuesto = (ingresos * 25) / 100
                            MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
                        Else
                            MsgBox ("Error el sacar valor")
                        End If
                    End If
                End If
            End If
        End If
    End If
End Sub

```

**Con condición dependiendo de**

```
Sub generadorImpuestos()
    MsgBox ("Bienvenido a IDAN")
    ingresos = Int(InputBox("Digite sus ingresos anuales"))
    Select Case ingresos
    Case Is < 0
        MsgBox ("Error al sacar calculo")
    Case 0 To 1000
        MsgBox ("No debe pagar impuestos")
    Case 1001 To 10000
        impuesto = (ingresos * 5) / 100
        MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
    Case 10001 To 100000
        impuesto = (ingresos * 10) / 100
        MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
    Case 100001 To 1000000
        impuesto = (ingresos * 15) / 100
        MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
    Case 1000001 To 10000000
        impuesto = (ingresos * 20) / 100
        MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
    Case Else
        impuesto = (ingresos * 25) / 100
        MsgBox ("Debe pagar $" & impuesto & (" de impuesto"))
    End Select
End Sub
```

**Algoritmo con select case**

![Algoritmo select case](https://i.imgur.com/53Yf34y.jpg)

**Diagrama de flujo de select case**

![Diagrama select case](https://i.imgur.com/dXdHGMj.jpg)

## Indice

[1. Trimestre 1] (/trimestre1)

[1.1 Hoja de vida] (/trimestre1/README.md)