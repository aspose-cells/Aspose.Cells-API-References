---
title: "Validation.Value2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation‑Eigenschaft. Stellt den zweiten Wert dar, der mit der Datenvalidierung verknüpft ist"
type: docs
url: /de/net/aspose.cells/validation/value2/
---
## Validation.Value2 property

Stellt den zweiten Wert dar, der mit der Datenvalidierung verknüpft ist.

```csharp
public object Value2 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ValidationCollection validations = worksheet.Validations;
            int index = validations.Add(CellArea.CreateCellArea(0, 0, 1, 1));
            Validation validation = validations[index];
            
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "-1000";
            validation.Formula2 = "1000";
            
            Console.WriteLine("Validation Value1: " + validation.Value1);
            Console.WriteLine("Validation Value2: " + validation.Value2);
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


