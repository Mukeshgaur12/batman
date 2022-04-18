import turtle
turtle.bgcolor("black")
t=turtle.Turtle()
t.speed(2000)
t.width(.0005)
t.goto(-250,-80)
t.goto(-250,80)
t.begin_fill()
t.width(5)
t.right(90)
t.circle(70,180)
t.goto(-110,80)
t.forward(100)
t.right(135)
t.forward(50)
t.left(45)
t.forward(60)
t.left(45)
t.forward(50)
t.right(135)
t.forward(100)
t.circle(70,180)
t.left(90)
t.circle(120,-180)
t.left(90)
t.circle(45,180)
t.left(185)
t.circle(60,180)
t.left(170)
t.circle(60,180)
t.left(185)
t.circle(45,180)
t.left(90)
t.circle(120,-180)
t.end_fill()   
turtle.speed(5)
turtle.pencolor('black')
r,g,b = 255, 0, 0
for i in range(255*2):
    turtle.colormode(255)
    if(i<255//3):
        g+=3
    elif(i<255*2//3):
        r-=3
    elif(i<255):
        b+=3
    elif(i<255*4//3):
        g-=3
    elif(i<255*5//3):
        r+=3
    else:
        b-=3
    turtle.fd(0)
    turtle.rt(0)
    turtle.bgcolor(r,g,b)
    t.pencolor("black")
turtle.done()
