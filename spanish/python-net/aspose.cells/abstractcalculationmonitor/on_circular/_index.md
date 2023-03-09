---
title: on_circular método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Implemente este método para hacer negocios al calcular fórmulas con referencias circulares.


###  Devoluciones

Si el motor de fórmulas necesita calcular esas celdas en circular después de esta llamada.
Es cierto para permitir que el motor de fórmulas continúe haciendo cálculos por ellos.
False para permitir que el motor de fórmulas simplemente marque esas celdas como Calculadas.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator |IEnumerator con elementos CalculationCell que representan celdas que<br/> dependen de las referencias circulares.|
###  Observaciones

En la implementación, el usuario también puede establecer el valor esperado como resultado calculado
para parte/todas esas celdas para que el motor de fórmulas no las calcule recursivamente.


###  Ver también
* módulo [aspose.cells](../../)
* clase [AbstractCalculationMonitor](/cells/es/python-net/aspose.cells/abstractcalculationmonitor)
