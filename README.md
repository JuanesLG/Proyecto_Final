# Proyecto_Final

```python
from turtle import *

# Inicializar la ventana de Turtle
ventana = Screen()
#ventana.setup(width=500, height=500)  # Establecer el tamaño de la ventana
ventana.title("Dibujo Turtle")

ventana.getcanvas().master.resizable(False, False)
ventana.getcanvas().master.iconbitmap(r"C:\Users\tortuga.ico")

ancho_ventana_turtle = 900
alto_ventana_turtle = 650

ancho_pantalla = ventana.getcanvas().master.winfo_screenwidth()
alto_pantalla = ventana.getcanvas().master.winfo_screenheight()
print(ancho_pantalla, alto_pantalla)


x = (ancho_pantalla - ancho_ventana_turtle) // 2
y = (alto_pantalla - alto_ventana_turtle) // 2

ventana.getcanvas().master.geometry(f"{ancho_ventana_turtle}x{alto_ventana_turtle}+{x-10}+{y-15}")



speed(10)


penup()
goto(-500,400)
pendown()
fillcolor("skyblue")
begin_fill()
for i in range(2):
 forward(1000)
 right(90)
 forward(400)
 right(90)
end_fill()

penup()
goto(-500,0)
pendown()

fillcolor("goldenrod")
begin_fill()
for i in range(2):
 forward(1000)
 right(90)
 forward(400)
 right(90)
end_fill()

penup()
goto(100,0)
pendown()

fillcolor("black")
begin_fill()
pensize(5)
forward(300)
left(126.87)
forward(125)
left(53.13)
forward(150)
left(53.13)
forward(125)
end_fill()

penup()
left(36.87)
pendown()
fillcolor("green")
begin_fill()
pensize(5)
for i in range(2):
 forward(150)
 left(90)
 forward(150)
end_fill()

pendown()
penup()
goto(285,-150)
pendown()
fillcolor("brown")
begin_fill()
forward(70)
left(90)
forward(70)
left(90)
forward(70)
end_fill()

penup()
goto(177.5, -25)
pendown()
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
goto(362.5, -25)
pendown()
fillcolor("white")
begin_fill()
left(90)
for i in range(4):
 forward(40)
 left(90)
end_fill()
forward(20)
left(90)
forward(40)
backward(20)
right(90)
forward(20)
backward(40)

penup()
goto(270,-120)
pendown()
pencolor("yellow")
fillcolor("yellow")
begin_fill()
width(1)
circle(4)
end_fill()


penup()
goto(-350,370)
pendown()
fillcolor("yellow")
begin_fill()
circle(70)
end_fill()

penup()
goto(-350,300)
pendown()
pencolor("yellow")
pensize(5)
for i in range(6):
 forward(100)
 backward(200)
 forward(100)
 right(30)

# Llamar a mainloop() para comenzar el ciclo principal de eventos de tkinter
ventana.mainloop()












```
