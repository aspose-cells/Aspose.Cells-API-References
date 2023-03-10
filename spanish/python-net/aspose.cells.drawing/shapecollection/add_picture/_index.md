---
title: add_picture método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 210
url: /es/python-net/aspose.cells.drawing/shapecollection/add_picture/
is_root: false
---
##  add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Agrega una imagen a la colección.


###  Devoluciones

[Picture](/cells/es/python-net/aspose.cells.drawing/picture) Objeto de imagen.


```python
def add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| lower_right_row | int | Índice de la fila inferior derecha|
| lower_right_column | int | Índice de la columna inferior derecha|
| stream | io.RawIOBase | Objeto de flujo que contiene los datos de la imagen.|

###  Ejemplo

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 0, 1, 0, fs)

```


##  add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Agrega una imagen a la colección.


###  Devoluciones

[Picture](/cells/es/python-net/aspose.cells.drawing/picture) Objeto de imagen.


```python
def add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| stream | io.RawIOBase | Objeto de flujo que contiene los datos de la imagen.|
| width_scale | int | Escala del ancho de la imagen, un porcentaje.|
| height_scale | int | Escala de altura de la imagen, un porcentaje.|

###  Ejemplo

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 1, fs, 50, 60)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
