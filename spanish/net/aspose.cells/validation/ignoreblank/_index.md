---
title: "Validation.IgnoreBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Indica si se permiten valores en blanco en la validación de datos del rango"
type: docs
url: /es/net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Indica si se permiten valores en blanco en la validación de datos del rango.

```csharp
public bool IgnoreBlank { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyIgnoreBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ValidationCollection validations = sheet.Validations;
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 1;
            area.StartColumn = 0;
            area.EndColumn = 1;
            Validation validation = validations[validations.Add(area)];

            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "2";
            validation.Formula2 = "20";
            validation.IgnoreBlank = true;

            Console.WriteLine("Validation created with IgnoreBlank set to: " + validation.IgnoreBlank);
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


