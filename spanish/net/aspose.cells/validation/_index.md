---
title: "Clase Validation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Validation. Representa data validation.settings"
type: docs
url: /es/net/aspose.cells/validation/
---
## Validation class

Representa la configuración de validación de datos.

```csharp
public class Validation
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Representa el estilo de alerta de validación. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Obtiene todos los [`CellArea`](../cellarea/) que contienen la configuración de validación de datos. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Representa el mensaje de error de validación de datos. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Representa el título del cuadro de diálogo de error de validación de datos. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Representa el valor o expresión asociado a la validación de datos. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Representa el valor o expresión asociado a la validación de datos. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Indica si se permiten valores en blanco en la validación de datos del rango. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Indica si la validación de datos muestra una lista desplegable que contiene valores aceptables. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Representa el mensaje de entrada de la validación de datos. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Representa el título del cuadro de diálogo de entrada de validación de datos. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Representa el operador de la validación de datos. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Indica si el mensaje de error de validación de datos se mostrará siempre que el usuario ingrese datos no válidos. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Indica si el mensaje de entrada de validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación de datos. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Representa el tipo de validación de datos. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Representa el primer valor asociado a la validación de datos. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Representa el segundo valor asociado a la validación de datos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Aplica la validación al área. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Aplica la validación al área. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Aplica la validación a las áreas dadas. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Copiar validación. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Obtiene el valor o expresión asociado con esta validación. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Obtiene el valor o expresión asociado con esta validación para una celda específica. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Obtiene el valor o expresión asociado con esta validación. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Obtiene el valor o expresión asociado con esta validación para una celda específica. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Obtenga el valor de la lista de validación para la celda especificada. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Obtenga el valor de la validación en la celda específica. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Elimine la configuración de validación en la celda. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Elimine la configuración de validación en el rango. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Elimina esta validación de las áreas dadas. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Establece el valor o expresión asociado con esta validación. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Establece el valor o expresión asociado con esta validación. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Defina un área de celdas para la validación
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Acceda a la colección de validaciones
            ValidationCollection validations = worksheet.Validations;

            // Agregue una nueva validación a la colección
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Establezca propiedades de validación
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // Guarda el libro de trabajo
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


