import turtle

t = turtle.Turtle()
t.speed(3)

# Head
t.penup()
t.goto(0, 50)
t.pendown()
t.color("#f2c197")
t.begin_fill()
t.circle(50)
t.end_fill()

# Hair
t.penup()
t.goto(0, 85)
t.pendown()
t.color("black")
t.begin_fill()
t.circle(50, 180)
t.end_fill()

# Eyes
t.penup()
t.goto(-20, 65)
t.pendown()
t.dot(10, "black")

t.penup()
t.goto(20, 65)
t.pendown()
t.dot(10, "black")

# Smile
t.penup()
t.goto(-20, 45)
t.pendown()
t.color("black")
t.width(3)
t.setheading(-60)
t.circle(25, 120)
# Body
t.penup()
t.goto(-40, 0)
t.pendown()
t.color("blue")
t.begin_fill()
for _ in range(2):
    t.forward(80)
    t.right(90)
    t.forward(100)
    t.right(90)
t.end_fill()

# Arms
t.penup()
t.goto(-40, -20)
t.pendown()
t.color("#f2c197")
t.width(10)
t.setheading(180)
t.forward(40)

t.penup()
t.goto(40, -20)
t.pendown()
t.setheading(0)
t.forward(40)

# Legs
t.penup()
t.goto(-20, -100)
t.pendown()
t.color("#333333")
t.setheading(-90)
t.forward(60)

t.penup()
t.goto(20, -100)
t.pendown()
t.setheading(-90)
t.forward(60)

t.hideturtle()
turtle.done()