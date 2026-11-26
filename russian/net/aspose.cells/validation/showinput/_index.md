---
title: "Validation.ShowInput"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Указывает, будет ли сообщение ввода проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных"
type: docs
url: /ru/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Указывает, будет ли вводное сообщение проверки данных отображаться каждый раз, когда пользователь выбирает ячейку в диапазоне проверки данных.

```csharp
public bool ShowInput { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать область проверки
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // Добавить проверку
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Установить свойство ShowInput
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // Сохраните книгу
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


