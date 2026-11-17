---
title: "Clase ConditionalFormattingValue"
linktitle: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase ConditionalFormattingValue. Encapsula el objeto que representa conditionalformattingvalue en Go."
type: docs
weight: 200
url: /es/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.

```go

type ConditionalFormattingValue struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetValue](./getvalue/) | Obtenga o establezca el valor de este objeto de valor de formato condicional. Debe usarse en conjunto con Type. |
| [SetValue](./setvalue/) | Obtenga o establezca el valor de este objeto de valor de formato condicional. Debe usarse en conjunto con Type. |
| [GetType](./gettype/) | Obtenga o establezca el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente \"Value\" a null. |
| [SetType](./settype/) | Obtenga o establezca el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente \"Value\" a null. |
| [IsGTE](./isgte/) | Obtenga o establezca la bandera Greater Than Or Equal. Use solo para conjuntos de iconos, determina si este valor umbral usa el operador mayor o igual. 'false' indica que se usa 'greater than' en lugar de 'greater than or equal to'. Valor predeterminado es true. |
| [SetIsGTE](./setisgte/) | Obtenga o establezca la bandera Greater Than Or Equal. Use solo para conjuntos de iconos, determina si este valor umbral usa el operador mayor o igual. 'false' indica que se usa 'greater than' en lugar de 'greater than or equal to'. Valor predeterminado es true. |
