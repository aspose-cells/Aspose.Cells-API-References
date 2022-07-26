---
title: Validation
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa validación de datos.configuración.
type: docs
weight: 6200
url: /es/net/aspose.cells/validation/
---
## Validation class

Representa validación de datos.configuración.

```csharp
public class Validation
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Representa el estilo de alerta de validación. |
| [Areas](../../aspose.cells/validation/areas) { get; } | Obtiene todos[`CellArea`](../cellarea) que contienen la configuración de validación de datos. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Representa el mensaje de error de validación de datos. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Representa el título del cuadro de diálogo de error de validación de datos. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Representa el valor o expresión asociada a la validación de datos. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Representa el valor o expresión asociada a la validación de datos. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Indica si la validación de datos de rango permite valores en blanco. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Representa el mensaje de entrada de validación de datos. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Representa el título del cuadro de diálogo de entrada de validación de datos. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Representa el operador para la validación de datos. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Indica si se mostrará el mensaje de error de validación de datos cada vez que el usuario ingrese datos no válidos. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Indica si el mensaje de entrada de validación de datos se mostrará cada vez que el usuario seleccione una celda en el rango de validación de datos. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Representa el tipo de validación de datos. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Representa el primer valor asociado a la validación de datos. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Representa el segundo valor asociado a la validación de datos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Aplica la validación al área. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Aplica la validación al área. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Aplica la validación a áreas dadas. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Copiar validación. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Obtiene el valor o expresión asociada a esta validación. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Obtiene el valor o la expresión asociada a esta validación para una celda específica. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Obtiene el valor o expresión asociada a esta validación. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Obtiene el valor o la expresión asociada a esta validación para una celda específica. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Obtener el valor de la lista de validación para la celda especificada. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Eliminar la configuración de validación en la celda. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Eliminar la configuración de validación en el rango. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Elimina esta validación de áreas dadas. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Establece el valor o expresión asociada a esta validación. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Establece el valor o expresión asociada a esta validación. |

### Ejemplos

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.WholeNumber
validation.Operator = OperatorType.Between
validation.Formula1 = "3"
validation.Formula2 = "1234"
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
