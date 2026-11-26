---
title: "Validation.ShowInput"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Indica si el mensaje de entrada de la validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación de datos"
type: docs
url: /es/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Indica si el mensaje de entrada de validación de datos se mostrará siempre que el usuario seleccione una celda en el rango de validación de datos.

```csharp
public bool ShowInput { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un área de validación
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // Agregar validación
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Establecer la propiedad ShowInput
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // Guarda el libro de trabajo
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


