---
title: "Validation.IgnoreBlank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Validation özelliği. Aralık veri doğrulaması tarafından boş değerlerin izin verilip verilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Aralık veri doğrulamasının boş değerleri izin verip vermediğini gösterir.

```csharp
public bool IgnoreBlank { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


