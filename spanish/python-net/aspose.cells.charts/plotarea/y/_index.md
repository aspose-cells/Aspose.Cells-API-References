---
title: y propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 280
url: /es/python-net/aspose.cells.charts/plotarea/y/
is_root: false
---
##  y propiedad

Obtiene u obtiene la coordenada y de la esquina superior superior del cuadro delimitador del área de trazado en unidades de 1/4000 del área del gráfico.

###  Observaciones

El cuadro delimitador del área de trazado incluye el área de trazado, las marcas de verificación (etiquetas de verificación) y un pequeño borde alrededor de las marcas de verificación.
 Si MS Excel no crea el valor, llame al método Chart.Calculate() antes de llamar a este método.


 El**X**, **Y** , **Ancho** y**Altura** de**Área de parcela** representa el área de la parcela
 Un cuadro delimitador que incluye el área de trazado, marcas de graduación (etiquetas de graduación) y un pequeño borde alrededor de las marcas de graduación.
 Si desea obtener el tamaño real del área de la trama, debe llamar**X interior** , **Y interior** , **Ancho interior** y
**Altura interior** propiedades.


Para Excel 2007 o posterior, el valor predeterminado es cero.
###  Definición:
```python
@property
def y(self):
    ...
@y.setter
def y(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [PlotArea](/cells/es/python-net/aspose.cells.charts/plotarea)
