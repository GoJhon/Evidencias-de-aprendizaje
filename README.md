# Evidencias-de-aprendizaje
Anotaciones de actividades en ADSO Sena








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

[1. Trimestre 1](/trimestre1)

[1.1 Hoja de vida](/trimestre1/hojaVida/README.md)

[1.2 Introducción a Visual Basic](/trimestre1/introduccionVisualBasic/README.md)

[1.3 Kanban, asignación de variables y concatenación](/trimestre1/kanbanAsignacionVarConcatenacion/README.md)

[1.4 Github desktop y condicionales](/trimestre1/githubDesktopCondicionales/README.md)

[1.5 Desafío grupal](/trimestre1/desafioGrupal/README.md)


