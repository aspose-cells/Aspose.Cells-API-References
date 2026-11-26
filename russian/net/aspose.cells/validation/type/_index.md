---
title: "Validation.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет тип проверки данных"
type: docs
url: /ru/net/aspose.cells/validation/type/
---
## Validation.Type property

Представляет тип проверки данных.

```csharp
public ValidationType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку в ячейку A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Продемонстрировать свойство Type
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Сохраните книгу
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### См. также

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


