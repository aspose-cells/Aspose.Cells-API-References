---
title: "Validation.InputTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет заголовок диалогового окна ввода проверки данных"
type: docs
url: /ru/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Представляет заголовок диалогового окна ввода проверки данных.

```csharp
public string InputTitle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объект проверки
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Установить диапазон проверки
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Установить свойства проверки
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Установить свойства входного сообщения
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Сохраните книгу
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // Проверить свойство InputTitle
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


