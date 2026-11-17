---
title: "PivotShowValuesSetting Clase"
linktitle: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase PivotShowValuesSetting. Encapsula el objeto que representa pivotshowvaluessetting en Go."
type: docs
weight: 200
url: /es/go-cpp/pivotshowvaluessetting/
---

## PivotShowValuesSetting class

Represents the settings about showing values as when the ShowDataAs calculation is in use.

```go

type PivotShowValuesSetting struct  {
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
| [GetCalculationType](./getcalculationtype/) | Representa cómo mostrar los valores de un campo de datos en el informe pivot. |
| [SetCalculationType](./setcalculationtype/) | Representa cómo mostrar los valores de un campo de datos en el informe pivot. |
| [GetBaseFieldIndex](./getbasefieldindex/) | Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso. |
| [SetBaseFieldIndex](./setbasefieldindex/) | Representa el campo base para un cálculo ShowDataAs cuando el cálculo ShowDataAs está en uso. |
| [GetBaseItemPositionType](./getbaseitempositiontype/) | Representa el tipo del elemento pivot base en el campo base cuando el cálculo ShowDataAs está en uso. Válido solo para campos de datos. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, por favor establezca el atributo PivotField.BaseItemIndex. |
| [SetBaseItemPositionType](./setbaseitempositiontype/) | Representa el tipo del elemento pivot base en el campo base cuando el cálculo ShowDataAs está en uso. Válido solo para campos de datos. Debido a que PivotItemPosition.Custom es solo de lectura, si necesita establecer PivotItemPosition.Custom, por favor establezca el atributo PivotField.BaseItemIndex. |
| [GetBaseItemIndex](./getbaseitemindex/) | Representa el índice personalizado del elemento pivot en el campo base cuando el cálculo ShowDataAs está en uso. Válido solo para campos de datos. |
| [SetBaseItemIndex](./setbaseitemindex/) | Representa el índice personalizado del elemento pivot en el campo base cuando el cálculo ShowDataAs está en uso. Válido solo para campos de datos. |
