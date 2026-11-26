---
title: "Validation.InputMessage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет вводное сообщение проверки данных"
type: docs
url: /ru/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Представляет вводное сообщение проверки данных.

```csharp
public string InputMessage { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать проверку
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Установить свойства входного сообщения
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Сохраните книгу
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


