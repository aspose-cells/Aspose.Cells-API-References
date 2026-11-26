---
title: "Перечисление ValidationAlertType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ValidationAlertType. Представляет стиль оповещения проверки данных"
type: docs
url: /ru/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Представляет стиль оповещения проверки данных.

```csharp
public enum ValidationAlertType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Information | `0` | Стиль информационного оповещения. |
| Stop | `1` | Стиль оповещения «Стоп». |
| Warning | `2` | Стиль предупреждающего оповещения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Определите область ячеек для проверки
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Добавить проверку на листе
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Установить свойства проверки
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Сохраните книгу
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


