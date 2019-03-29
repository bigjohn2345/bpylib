'''
renderShape(ShapeType{int},xPosition{int},yPosition{int},shapeData{array})

shape types:
1-circle
2-square
3-triangle

Shape Data Types:
0-circle radius {int}
1-polygon side length {int}
2-line thickness {string}
3-shape color {string}
'''

def renderShape(type,sPosX,sPosY,shapeData):
    if shapeData[2] is not None:
        pensize(shapeData[2])
    if shapeData[3] is not None:
        color(shapeData[3])
    if type==1:
        setposition(sPosX,sPosY)
        pendown()
        circle(shapeData[0])
        penup()
    if type==2:
        setposition(sPosX-(shapeData[1]/2),sPosY)
        pendown()
        for i in range(0,4):
            forward(shapeData[1])
            left(90)
        penup()
    if type==3:
        setposition(sPosX-(shapeData[1]/2),sPosY)
        for i in range(0,3):
            forward(shapeData[1])
            left(120)
