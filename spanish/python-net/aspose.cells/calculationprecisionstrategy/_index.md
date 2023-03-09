---
title: CalculationPrecisionStrategy enumeración
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1820
url: /es/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
##  CalculationPrecisionStrategy enumeración
Enumera estrategias para manejar la precisión del cálculo.
Debido al problema de precisión de la aritmética de coma flotante IEEE 754, es posible que algunas fórmulas "aparentemente simples" no se calculen como el resultado esperado.
Como la fórmula "=-0.45+0.43+0.02", cuando se calculan los operandos directamente con el operador '+', el resultado no es cero.
algunas estrategias especiales pueden dar el resultado esperado.



El tipo CalculationPrecisionStrategy expone los siguientes miembros:

###  Campos
| Campo| Descripción|
| :- | :- |
| NONE | No se aplicó ninguna estrategia en el cálculo.<br/>Al calcular, simplemente use el valor doble original como operando y devuelva el resultado directamente.<br/> Más eficiente para el rendimiento y aplicable para la mayoría de los casos.|
| ROUND | Redondea el resultado del cálculo según dígitos significativos.|
| DECIMAL | Usa decimales como operandos cuando es posible.<br/> Más ineficiente para el rendimiento.|



###  Ver también
* módulo [aspose.cells](..)
