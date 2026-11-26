---
title: "Validation.IgnoreBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Указывает, разрешены ли пустые значения в проверке данных диапазона"
type: docs
url: /ru/net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Указывает, разрешены ли пустые значения в проверке диапазона данных.

```csharp
public bool IgnoreBlank { get; set; }
```

### Примеры

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

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


