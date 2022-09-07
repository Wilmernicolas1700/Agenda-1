# Agenda

### Dia 12/08/22
Programacion general con el instructor Henry guzman

``` 
sub sena

nom = "luis"
num = "10"
nom = "maria"

end sena

Programación general
sub sena

nom = "Luis" num = "10" nom = "María"
``` 

acabar con sena


### Dia 19/08/22

Sub Suma() a = Int(InputBox("Digitar el numero para la variable a")) b = Int(InputBox("Digitar el numero para la variable b"))

c = a + b

MsgBox "El resultado es:" & c
Finalizar sub

### Dia 24/08/22

ingrese el nombre de un alumno y las notas de un examen parcial, examen final y el promedio de practicas; muestre el nombre del alumno y su promedio final solo si el alumno está aprobado,tenga en cuenta que para el calculo del promedio la nota del examen final tiene peso doble

End Sub

### Dia 26/08/22

Ejercicio de ingreo anual
``` 
sub prueba () 

ingresoanual = InputBox("Ingresa su ingreso anual: ")

If ingresoanual < 1000 Then
 MsgBox ("no hay impuesto")
Else
    If ingresoanual >= 1001 And ing < 10000 Then
        total = ingresoanual * 0.05
        MsgBox ("El total a pagar es: ") & total
    Else
        If ingresoanual >= 10001 And ing < 100000 Then
        total = ingresoanual * 0.10
        MsgBox ("El total a pagar es: ") & total
	
        Else
             If ingresoanual >= 100001 And ing < 1000000 Then
             total = ingresoanual * 0.15
             MsgBox ("El total a pagar es: ") & total
	      
            Else
                If ingresoanual >= 1000001 And ing < 10000000 Then
                total = ingresoanual * 0.20
                MsgBox ("El total a pagar es: ") & total
		
		Else
                    If ingresoanual > 10000001 Then
                    total = ingresoanual * 0.25
                    MsgBox ("El total a pagar es: ") & total
		    
                End If
            End If
        End If
    End If
End If

``` 

### Dia 28/08/22

``` 
Sub inicio()
    
    abono = 0
    no_abono = 0
    cant = 0
    recaudo_total = 0
    
    For c = 1 To 3
        pregunta = InputBox("Desea aportar para la recolecta (si o no")
        If pregunta = "si" Then
            abono = abono + 1
            dinero_rec = Int(InputBox("que cantidad va a aportar?"))
            recaudo_total = recaudo_total + dinero_rec
            If dinero_rec >= 10000 Then
                cant = cant + 1
            End If
        Else
            no_abono = no_abono + 1
        End If
    Next c
    
    prom = recaudo_total / abono
    MsgBox "El total de recaudado por los estudiantes es: " & recaudo_total
    MsgBox "El promedio recaudado por estudiante es: " & prom
    MsgBox "El numero de estudiantes que aportaron es: " & "(" & abono & ")" & " Estudiantes"
    MsgBox "El numero de estudiantes que no aportaron es: " & "(" & no_abono & ")" & " Estudiantes"
    MsgBox "Los estudiantes que aportaron una cantidad superior a $10.000: " & "(" & cant & ")" & " Estudiantes"
        
End Sub
``` 

### Dia 29/08/2022

Crear un registro
``` 
Sub almacenar()
    fila = datos.Cells(1, 7)
    datos.Cells(fila, 1) = formulario.Cells(7, 4)
    datos.Cells(fila, 2) = formulario.Cells(9, 4)
    datos.Cells(fila, 3) = formulario.Cells(11, 4)
    datos.Cells(fila, 4) = formulario.Cells(13, 4)
    MsgBox ("los datos se guardaron correctamente")
    datos.Cells(1, 7) = fila + 1
End Sub

Registro


Sub sena()
    For x = 1 To 15
    Z = InputBox(" ingrese un nombre")
    fila = Hoja1.Cells(1, 7)
    Hoja1.Cells(fila, 2) = Z
    Hoja1.Cells(1, 7) = fila + 1
    Next x
End Sub
``` 

## 02/09/2022
Ejercicio con Len y Mid


Sub nombres()
    For x = 2 To 21
        nombre = Nom.Cells(x, 1)
        ulti = Len(nombre) - 1
        Nom.Cells(x, 2) = Mid(nombre, ulti, 2)
    Next x
End Sub
 
Ejercicio #2


Sub nombres()
    For x = 2 To 21
    nombre = Nom.Cells(x, 1)
    año = Nom.Cells(x, 2)
    municipio = Nom.Cells(x, 3)
    ulti = Len(municipio) - 1
    Nom.Cells(x, 4) = Mid(año, 1, 2) & Mid(municipio, ulti, 2) & Mid(nombre, 1, 2)
    Next x
End Sub