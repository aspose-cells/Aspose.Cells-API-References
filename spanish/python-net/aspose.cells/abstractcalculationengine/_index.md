---
title: AbstractCalculationEngine clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  AbstractCalculationEngine clase
Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.



El tipo AbstractCalculationEngine expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_param_literal_required](/cells/es/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Indica si este motor necesita el texto literal del parámetro mientras realiza el cálculo. El valor predeterminado es falso.|
| [process_built_in_functions](/cells/es/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Si esta implementación debe verificar y procesar las funciones integradas que han sido compatibles con el motor integrado.<br/>El valor predeterminado es falso.<br/> Si el usuario necesita cambiar la lógica de cálculo de algunas funciones integradas, esta propiedad debe establecerse como verdadera.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [calculate(data)](/cells/es/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Calcula una función con datos dados.|



###  Observaciones

El usuario no debe modificar ninguna parte del libro de trabajo directamente en esta implementación (excepto el resultado calculado de la función personalizada, que se puede configurar mediante la propiedad CalculationData.CalculatedValue).
De lo contrario, se puede producir un resultado inesperado o una excepción.
Si el usuario necesita cambiar otros datos además del resultado calculado en la implementación de algunas funciones personalizadas,
por ejemplo, cambiar la fórmula, el estilo, etc. de la celda, el usuario debe recopilar esos datos en esta implementación y cambiarlos fuera del alcance del cálculo de la fórmula.

###  Ver también
* módulo [aspose.cells](..)
