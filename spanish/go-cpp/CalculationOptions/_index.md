---
title: "Clase CalculationOptions"
linktitle: "CalculationOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase CalculationOptions. Encapsula el objeto que representa calculationoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/calculationoptions/
---

## CalculationOptions class

Represents options for calculation.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetIgnoreError](./getignoreerror/) | Indica si los errores encontrados al calcular fórmulas deben ser ignorados.El error puede ser una función no compatible, enlaces externos, etc.El valor predeterminado es verdadero. |
| [SetIgnoreError](./setignoreerror/) | Indica si los errores encontrados al calcular fórmulas deben ser ignorados.El error puede ser una función no compatible, enlaces externos, etc.El valor predeterminado es verdadero. |
| [GetRecursive](./getrecursive/) | Indica si se calculan las celdas dependientes de forma recursiva al calcular una celda que depende de otras celdas.El valor predeterminado es verdadero. |
| [SetRecursive](./setrecursive/) | Indica si se calculan las celdas dependientes de forma recursiva al calcular una celda que depende de otras celdas.El valor predeterminado es verdadero. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Indica si el usuario ha especificado explícitamente el comportamiento de actualizar fórmulas de matriz dinámica antes de calcular fórmulas especificadas. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Indica si las fórmulas de matriz dinámica deben actualizarse antes de calcular fórmulas. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Indica si las fórmulas de matriz dinámica deben actualizarse antes de calcular fórmulas. |
| [GetCustomEngine](./getcustomengine/) | El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [SetCustomEngine](./setcustomengine/) | El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells. |
| [GetCalcStackSize](./getcalcstacksize/) | El tamaño de la pila para calcular celdas de forma recursiva. El valor predeterminado es 200. |
| [SetCalcStackSize](./setcalcstacksize/) | El tamaño de la pila para calcular celdas de forma recursiva. El valor predeterminado es 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | Especifica la estrategia para procesar la precisión del cálculo. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | Especifica la estrategia para procesar la precisión del cálculo. |
| [GetLinkedDataSources](./getlinkeddatasources/) | Especifica las fuentes de datos para enlaces externos utilizados en fórmulas. |
| [SetLinkedDataSources](./setlinkeddatasources/) | Especifica las fuentes de datos para enlaces externos utilizados en fórmulas. |
| [GetCharacterEncoding](./getcharacterencoding/) | Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas.Para funciones como CHAR, CODE, el resultado calculado depende de la configuración regional y del conjunto de caracteres predeterminado del entorno.Con esta propiedad el usuario puede especificar la codificación adecuada utilizada para esas funciones para obtener el resultado esperado. |
| [SetCharacterEncoding](./setcharacterencoding/) | Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas.Para funciones como CHAR, CODE, el resultado calculado depende de la configuración regional y del conjunto de caracteres predeterminado del entorno.Con esta propiedad el usuario puede especificar la codificación adecuada utilizada para esas funciones para obtener el resultado esperado. |
