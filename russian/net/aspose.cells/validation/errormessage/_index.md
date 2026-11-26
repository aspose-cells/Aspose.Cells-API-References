---
title: "Validation.ErrorMessage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Представляет сообщение об ошибке проверки данных"
type: docs
url: /ru/net/aspose.cells/validation/errormessage/
---
## Validation.ErrorMessage property

Представляет сообщение об ошибке проверки данных.

```csharp
public string ErrorMessage { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorMessageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать проверку для ячейки A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";

            // Установить свойства сообщения об ошибке
            validation.ErrorMessage = "Value must be between 10 and 20";
            validation.ErrorTitle = "Invalid Input";
            validation.AlertStyle = ValidationAlertType.Stop;

            // Применить проверку и протестировать её
            worksheet.Cells["A1"].PutValue(5); // Invalid value
            Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);

            // Сохраните книгу
            workbook.Save("ValidationErrorMessageDemo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


