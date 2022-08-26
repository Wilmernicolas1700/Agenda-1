# Agenda


### Dia 12/08/22

### Programacion general con el instructor Henry guzman

sub sena

nom = "luis"
num = "10"
nom = "maria"

end sena

Programación general
sub sena

nom = "Luis" num = "10" nom = "María"

acabar con sena

### Dia 19/08/22

Sub Suma() a = Int(InputBox("Digitar el numero para la variable a")) b = Int(InputBox("Digitar el numero para la variable b"))

c = a + b

MsgBox "El resultado es:" & c

Finalizar sub

### Dia 24/08/22 

Actividad en clase 

precio<- 100
escribir "Digite el numero de noches"
leer noches

total <- precio * noches

si noches > 3 entonces 
	descuento <- total*.05
	
	 escribir "Su pago total es: ", total - descuento 
sino 
	
	escribir "su pago total sin descuento es: ", total
	
	
FinSi

### Dia 24/08/22

ingrese el nombre de un alumno y las notas de un examen parcial, examen final y el promedio de practicas; muestre el nombre del alumno y su promedio final solo si el alumno está aprobado,tenga en cuenta que para el calculo del promedio la nota del examen final tiene peso doble

definir alumno como caracter 
definir examenp, examenf, promediop como real
definir promediofinal Como Real

     escribir "por favor digite el nombre del alumno" 
      leer alumno 

Escribir "Las notas seran calificadas de 1 a 5" 

Escribir "Digite la calificacion del examen parcial"
    leer examenp
Escribir "Digite la calificacion del examen final"
    leer examenf
Escribir "Digite la calificacion del promedio de practicas"
    leer promediop

final <- (examenp+promediop+(examenf*2))/3

si final > 3 entonces 

	escribir "Estudiante aprobado: ", alumno 
	escribir "su promedio es de: ", final 
sino 
	
	escribir alumno, " Estudiante no aprobado"
	escribir "su promedio general es de: ", final 
	
FinSi
