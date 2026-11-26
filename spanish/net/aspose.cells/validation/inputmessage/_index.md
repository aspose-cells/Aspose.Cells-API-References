---
title: "Validation.InputMessage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Representa el mensaje de entrada de la validación de datos"
type: docs
url: /es/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Representa el mensaje de entrada de la validación de datos.

```csharp
public string InputMessage { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear validación
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Establecer las propiedades del mensaje de entrada
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Guarda el libro de trabajo
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


