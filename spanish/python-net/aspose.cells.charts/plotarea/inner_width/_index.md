---
title: inner_width propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 160
url: /es/python-net/aspose.cells.charts/plotarea/inner_width/
is_root: false
---
##  inner_width propiedad

Obtiene o establece el ancho del área de trazado en unidades de 1/4000 del área del gráfico.

###  Observaciones

El cuadro delimitador del área de trazado incluye el área de trazado, las marcas de verificación (etiquetas de verificación) y un pequeño borde alrededor de las marcas de verificación.
 Si MS Excel no crea el valor, llame al método Chart.Calculate() antes de llamar a este método.


 El**X**, **Y** , **Ancho** y**Altura** de**Área de Parcela** representa el área de la parcela
 cuadro delimitador que incluye el área de trazado, marcas de graduación (etiquetas de graduación) y un pequeño borde alrededor de las marcas de graduación.
 Si desea obtener el tamaño real del área de la trama, debe llamar**InteriorX** , **interiorY** , **Ancho interior** y
**Altura interior** propiedades.


Para Excel 2007 o posterior, el valor predeterminado es cero. debe llamar a obtener el valor después de llamar a Chart.Calculate().
###  Definición:
```python
@property
def inner_width(self):
    ...
@inner_width.setter
def inner_width(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [PlotArea](/cells/es/python-net/aspose.cells.charts/plotarea)
