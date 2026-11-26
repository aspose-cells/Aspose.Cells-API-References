---
title: "Validation.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Representa el tipo de validación de datos"
type: docs
url: /es/net/aspose.cells/validation/type/
---
## Validation.Type property

Representa el tipo de validación de datos.

```csharp
public ValidationType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una validación a la celda A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Demostrar la propiedad Type
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### Ver también

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


