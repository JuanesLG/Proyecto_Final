# Proyecto_Final

```python
from turtle import *

ventana = Screen()
ventana.title("Paisaje")

ventana.getcanvas().master.resizable(False, False)
ventana.getcanvas().master.iconbitmap("G.ico")

ancho_ventana_turtle = 800
alto_ventana_turtle = 600

ancho_pantalla = ventana.getcanvas().master.winfo_screenwidth()
alto_pantalla = ventana.getcanvas().master.winfo_screenheight()


x = (ancho_pantalla - ancho_ventana_turtle) // 2
y = (alto_pantalla - alto_ventana_turtle) // 2

ventana.getcanvas().master.geometry(f"{ancho_ventana_turtle}x{alto_ventana_turtle}+{x}+{y}")

speed (10)

def posicion_cielo():
 penup()
 goto(-500,400)
 pendown()

def cielo():
 fillcolor("skyblue")
 begin_fill()
 for i in range(2):
  forward(1000)
  right(90)
  forward(400)
  right(90)
 end_fill()


def posicion_suelo():
 penup()
 goto(-500,0)
 pendown()

def suelo():
 fillcolor("seaGreen")
 begin_fill()
 for i in range(2):
  forward(1000)
  right(90)
  forward(400)
  right(90)
 end_fill()

def posicion_casa():
    penup()
    goto(50,0)

def frente_casa():
    fillcolor("firebrick")
    begin_fill()
    for i in range (2):
        pendown()
        forward(300)
        right(90)
        forward(150)
        right(90)
    end_fill()

def techo_casa():
    fillcolor("black")
    begin_fill()
    forward(300)
    left(126.87)
    forward(125)
    left(53.13)
    forward(150)
    left(53.13)
    forward(125)
    end_fill()
    left(126.87)

def posicion_ventana_1():
 penup()
 goto(105,-25)
 pendown()

def posicion_ventana_2():
 penup()
 goto(257.5,-25)
 pendown() 

def ventanas():
 fillcolor("white")
 begin_fill()
 for i in range(4):
  forward(40)
  right(90)
 end_fill()
 forward(20)
 right(90)
 forward(40)
 backward(20)
 right(90)
 forward(20)
 backward(40)
 penup()
 forward(40)
 right(90)
 forward(20)
 right(90)

def posicion_puerta():
 penup()
 goto(230,-150)
 pendown()
  

def puerta_y_chapa():
 fillcolor("maroon")
 begin_fill()
 for i in range(2):
  left(90)
  forward(70)
  left(90)
  forward(60)
 end_fill()

 penup()
 goto(220,-120)
 pendown()
 pencolor("yellow")
 fillcolor("yellow")
 begin_fill()
 width(1)
 circle(4)
 end_fill()

def sol():
    penup()
    goto(-250,220)
    pendown()
    pencolor('orange')
    pensize(5)

    for i in range(6):
       forward(80)
       back(160)
       forward(80)
       right(30)

    penup()
    goto(-250,270)
    pendown()
    fillcolor('yellow') 
    begin_fill()
    circle(50)
    end_fill()



posicion_cielo()
cielo()
posicion_suelo()
suelo()
posicion_casa()
frente_casa()
techo_casa()
posicion_ventana_1()
ventanas()
posicion_ventana_2()
ventanas()
posicion_puerta()
puerta_y_chapa()
sol()

ventana.mainloop()












```
