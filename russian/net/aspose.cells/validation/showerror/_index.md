---
title: "Validation.ShowError"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные"
type: docs
url: /ru/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Указывает, будет ли сообщение об ошибке проверки данных отображаться каждый раз, когда пользователь вводит недопустимые данные.

```csharp
public bool ShowError { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать проверку для ячейки A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Установить свойства проверки
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Настройте оповещение об ошибке
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Создайте ещё одну проверку, чтобы продемонстрировать копирование свойств
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // Скопируйте ShowError и связанные свойства из первой проверки
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Сохраните книгу
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


