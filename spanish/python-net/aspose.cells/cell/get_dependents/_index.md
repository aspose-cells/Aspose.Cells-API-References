---
title: get_dependents método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 90
url: /es/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
Obtenga todas las celdas cuya fórmula hace referencia directamente a esta celda.



```python
def get_dependents(self, is_all):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| is_all | bool | Indica si verificar fórmulas en otras hojas de trabajo|
###  Observaciones

* Si una referencia que contiene esta celda aparece en la fórmula de una celda, esa celda se tomará como

el dependiente de esta celda, sin importar la referencia o si esta celda se usa o no durante el cálculo.
Por ejemplo, aunque la celda A2 en la fórmula "=SI(VERDADERO,A1,A2)" no se usa al calcular,
Esta fórmula todavía se toma como dependiente de A2.
Para obtener las fórmulas cuyos resultados calculados dependen de esta celda, utilice [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation). Al rastrear los dependientes de una celda, se analizarán y comprobarán todas las fórmulas del libro de trabajo o de la hoja de trabajo.
Por lo tanto, es un proceso que consume mucho tiempo. Si el usuario necesita rastrear dependientes para muchas celdas, usar este método
causar un rendimiento deficiente. Para considerar el rendimiento, el usuario debe usar [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation) en su lugar.
O bien, el usuario puede recopilar un mapa de precedentes de todas las celdas por [Cell.get_precedents()](/cells/es/python-net/aspose.cells/cell/get_precedents) en primer lugar,
y luego construya el mapa de dependientes de acuerdo con el mapa de precedentes.

* Si una referencia que contiene esta celda aparece en la fórmula de una celda, esa celda se tomará como
el dependiente de esta celda, sin importar la referencia o si esta celda se usa o no durante el cálculo.
Por ejemplo, aunque la celda A2 en la fórmula "=SI(VERDADERO,A1,A2)" no se usa al calcular,
Esta fórmula todavía se toma como dependiente de A2.
Para obtener las fórmulas cuyos resultados calculados dependen de esta celda, utilice [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation). Al rastrear los dependientes de una celda, se analizarán y comprobarán todas las fórmulas del libro de trabajo o de la hoja de trabajo.
Por lo tanto, es un proceso que consume mucho tiempo. Si el usuario necesita rastrear dependientes para muchas celdas, usar este método
causar un rendimiento deficiente. Para considerar el rendimiento, el usuario debe usar [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation) en su lugar.
O bien, el usuario puede recopilar un mapa de precedentes de todas las celdas por [Cell.get_precedents()](/cells/es/python-net/aspose.cells/cell/get_precedents) en primer lugar,
y luego construya el mapa de dependientes de acuerdo con el mapa de precedentes.

* Si una referencia que contiene esta celda aparece en la fórmula de una celda, esa celda se tomará como
el dependiente de esta celda, sin importar la referencia o si esta celda se usa o no durante el cálculo.
Por ejemplo, aunque la celda A2 en la fórmula "=SI(VERDADERO,A1,A2)" no se usa al calcular,
Esta fórmula todavía se toma como dependiente de A2.
Para obtener las fórmulas cuyos resultados calculados dependen de esta celda, utilice [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation). Al rastrear los dependientes de una celda, se analizarán y comprobarán todas las fórmulas del libro de trabajo o de la hoja de trabajo.
Por lo tanto, es un proceso que consume mucho tiempo. Si el usuario necesita rastrear dependientes para muchas celdas, usar este método
causar un rendimiento deficiente. Para considerar el rendimiento, el usuario debe usar [Cell.get_dependents_in_calculation(recursive)](/cells/es/python-net/aspose.cells/cell/get_dependents_in_calculation) en su lugar.
O bien, el usuario puede recopilar un mapa de precedentes de todas las celdas por [Cell.get_precedents()](/cells/es/python-net/aspose.cells/cell/get_precedents) en primer lugar,
y luego construya el mapa de dependientes de acuerdo con el mapa de precedentes.
###  Ejemplos

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cell](/cells/es/python-net/aspose.cells/cell)
