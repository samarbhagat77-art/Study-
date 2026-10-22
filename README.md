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