---
title: set_formulas método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells/formatcondition/set_formulas/
is_root: false
---
##  set_formulas(formula1, formula2, is_r1c1, is_local) {#str-str-bool-bool}
Establece el valor o la expresión asociada con esta condición de formato.



```python
def set_formulas(self, formula1, formula2, is_r1c1, is_local):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| formula1 | str | El valor o la expresión asociada con esta condición de formato.<br/>Si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario, se tomará como valor simple (texto, número, bool).<br/> Para el valor de texto que comienza con '=', el usuario puede ingresarlo como fórmula en formato: "=\"=...\"".|
| formula2 | str | El valor o la expresión asociada con esta condición de formato. El formato de entrada es el mismo con formula1|
| is_r1c1 | bool | Si la fórmula es la fórmula R1C1.|
| is_local | bool | Si la fórmula tiene formato de configuración regional.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [FormatCondition](/cells/es/python-net/aspose.cells/formatcondition)
