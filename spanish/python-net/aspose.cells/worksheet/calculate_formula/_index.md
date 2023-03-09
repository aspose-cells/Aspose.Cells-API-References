---
title: calculate_formula método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 80
url: /es/python-net/aspose.cells/worksheet/calculate_formula/
is_root: false
---
##  calculate_formula(formula) {#str}
Calcula una fórmula.


###  Devoluciones

Resultado de la fórmula calculada.


```python
def calculate_formula(self, formula):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| formula | str | Fórmula a calcular.|


##  calculate_formula(formula, opts) {#str-CalculationOptions}
Calcula una fórmula.


###  Devoluciones

Resultado de la fórmula calculada.


```python
def calculate_formula(self, formula, opts):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| formula | str | Fórmula a calcular.|
| opts | [CalculationOptions](/cells/es/python-net/aspose.cells/calculationoptions) | Opciones para calcular la fórmula|


##  calculate_formula(options, recursive) {#CalculationOptions-bool}
Calcula todas las fórmulas en esta hoja de cálculo.



```python
def calculate_formula(self, options, recursive):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| options | [CalculationOptions](/cells/es/python-net/aspose.cells/calculationoptions) | Opciones de cálculo|
| recursive | bool | Verdadero significa que si las celdas de la hoja de trabajo dependen de las celdas de otras hojas de trabajo,<br/>las celdas dependientes en otras hojas de cálculo también se calcularán.<br/> Falso significa que se han calculado todas las fórmulas de la hoja de trabajo y los valores son correctos.|


##  calculate_formula(recursive, ignore_error, custom_function) {#bool-bool-ICustomFunction}
Calcula todas las fórmulas en esta hoja de cálculo.



```python
def calculate_formula(self, recursive, ignore_error, custom_function):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| recursive | bool | Verdadero significa que si las celdas de la hoja de trabajo dependen de las celdas de otras hojas de trabajo,<br/>las celdas dependientes en otras hojas de cálculo también se calcularán.<br/> Falso significa que se han calculado todas las fórmulas de la hoja de trabajo y los valores son correctos.|
| ignore_error | bool | Indica si se oculta el error en el cálculo de fórmulas.<br/> El error puede ser funciones no compatibles, enlaces externos, etc.|
| custom_function | [ICustomFunction](/cells/es/python-net/aspose.cells/icustomfunction) | Las funciones de cálculo de fórmula personalizada para ampliar el motor de cálculo.|
###  Observaciones

NOTA: Este miembro ahora está obsoleto.
utilice el método CalculateFormula(CalculationOptions, bool).
 Este método se eliminará 12 meses después desde agosto de 2020.
Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Worksheet](/cells/es/python-net/aspose.cells/worksheet)
