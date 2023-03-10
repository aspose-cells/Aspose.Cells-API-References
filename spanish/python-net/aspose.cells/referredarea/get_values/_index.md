---
title: get_values método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/referredarea/get_values/
is_root: false
---
##  get_values() {#}
Obtiene valores de celda en esta área.


###  Devoluciones

Si esta área no es válida, "#REF!" Será devuelto;
Si esta área es una sola celda, devuelva el objeto de valor de celda;
De lo contrario, devuelva una matriz 2D para todos los valores en esta área.


```python
def get_values(self):
    ...
```




##  get_values(calculate_formulas) {#bool}
Obtiene valores de celda en esta área.


###  Devoluciones

Si esta área no es válida, "#REF!" Será devuelto;
Si esta área es una sola celda, devuelva el objeto de valor de celda;
De lo contrario, devuelva una matriz 2D para todos los valores en esta área.


```python
def get_values(self, calculate_formulas):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| calculate_formulas | bool | En este rango, si hay algunas fórmulas que no han sido calculadas,<br/> esta bandera indica si esas fórmulas deben calcularse recursivamente|



###  Ver también
* módulo [aspose.cells](../../)
* clase [ReferredArea](/cells/es/python-net/aspose.cells/referredarea)
