import turtle

rang=('orange', 'orange')
wn=turtle.Screen()
gr=turtle.Pen()
gr.hideturtle()


def Paint(repeat,color):
    turtle.bgcolor(color)
    global rang
    global gr
    for x in range(repeat):
        gr.pencolor(rang[x%2])
        gr.width(x/100+1)
        gr.pensize(5)
        gr.forward(x)
        gr.right(150)
        gr.speed(0)


Paint(400,"black")
wn.mainloop()
