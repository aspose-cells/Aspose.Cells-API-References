---
title: "Перечисление ValidationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ValidationType. Представляет тип проверки данных"
type: docs
url: /ru/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Представляет тип проверки данных.

```csharp
public enum ValidationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| AnyValue | `0` | Тип проверки любого значения. |
| WholeNumber | `1` | Тип проверки целого числа. |
| Decimal | `2` | Тип проверки десятичного числа. |
| List | `3` | Тип проверки списка. |
| Date | `4` | Тип проверки даты. |
| Time | `5` | Тип проверки времени. |
| TextLength | `6` | Тип проверки длины текста. |
| Custom | `7` | Тип пользовательской проверки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку на листе
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Установить тип проверки в WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Установить дополнительные свойства для проверки
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Сохраните книгу
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


