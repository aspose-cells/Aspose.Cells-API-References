---
title: set_two_color_gradient método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells.drawing/gradientfill/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
Establece el relleno especificado en un degradado de dos colores.
Solo aplica para Excel 2007.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Un color degradado.|
| color2 | aspose.pydrawing.Color | Dos degradados de color.|
| style | [GradientStyleType](/cells/es/python-net/aspose.cells.drawing/gradientstyletype) | Estilo de sombreado degradado.|
| variant | int |La variante degradada. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado en el cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2.|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
Establece el relleno especificado en un degradado de dos colores.
Solo aplica para Excel 2007.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Un color degradado.|
| transparency1 | float | El grado de transparencia del color1 como un valor de 0,0 (opaco) a 1,0 (transparente).|
| color2 | aspose.pydrawing.Color | Dos degradados de color.|
| transparency2 | float | El grado de transparencia del color2 como un valor de 0,0 (opaco) a 1,0 (transparente).|
| style | [GradientStyleType](/cells/es/python-net/aspose.cells.drawing/gradientstyletype) | Estilo de sombreado degradado.|
| variant | int |La variante degradada. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado en el cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2.|



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [GradientFill](/cells/es/python-net/aspose.cells.drawing/gradientfill)
