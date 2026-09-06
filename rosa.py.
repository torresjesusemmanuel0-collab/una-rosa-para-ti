import turtle
import math

# Configuración de la ventana
screen = turtle.Screen()
screen.bgcolor("#0d0d1a")
screen.title("Una rosa para ti ❤️")

t = turtle.Turtle()
t.speed(0)
t.hideturtle()

# Dibuja la flor (Rosa de Rodonea)
t.penup()
t.goto(0, 40)
t.pendown()

for i in range(360 * 5):
    theta = math.radians(i)
    # Ecuación paramétrica de pétalos superpuestos
    r = 150 * math.sin(5/2 * theta)
    x = r * math.cos(theta)
    y = r * math.sin(theta) + 40
    
    # Cambio progresivo de color (rojo a magenta)
    color_val = abs(math.sin(theta))
    t.pencolor(1.0, 0.1 * color_val, 0.3 + 0.4 * color_val)
    t.goto(x, y)

# Tallo
t.penup()
t.goto(0, -110)
t.pendown()
t.pencolor("#2b9348")
t.pensize(4)
t.setheading(270)
t.circle(200, 30)

# Hoja izquierda
t.pensize(2)
t.fillcolor("#55a630")
t.begin_fill()
t.circle(50, 70)
t.left(110)
t.circle(50, 70)
t.end_fill()

# Dedicatoria
t.penup()
t.goto(0, -230)
t.pencolor("#ff758f")
t.write("Una rosa que nunca se marchita, para ti. ❤️", align="center", font=("Arial", 13, "bold"))

turtle.done()
