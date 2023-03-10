---
title: set_one_color_gradient método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.drawing/lineformat/set_one_color_gradient/
is_root: false
---
##  set_one_color_gradient(color, degree, style, variant) {#aspose.pydrawing.Color-float-GradientStyleType-int}
Establece el relleno especificado en un degradado de un color.
Solo aplica para Excel 2007.



```python
def set_one_color_gradient(self, color, degree, style, variant):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Un color degradado.|
| degree | float | El grado de gradiente. Puede ser un valor de 0,0 (oscuro) a 1,0 (claro).|
| style | [GradientStyleType](/cells/es/python-net/aspose.cells.drawing/gradientstyletype) | Estilo de sombreado degradado.|
| variant | int |La variante degradada. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado en el cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2.|



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [LineFormat](/cells/es/python-net/aspose.cells.drawing/lineformat)
