---
title: "Cell.GetValidationValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает значение проверки, примененной к этой ячейке"
type: docs
url: /ru/net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Получает значение проверки, примененной к этой ячейке.

```csharp
public bool GetValidationValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationValueDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон проверки
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.TextLength;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "5";

            // Примените проверку к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            validation.AddArea(new CellArea { StartRow = cell.Row, StartColumn = cell.Column, EndRow = cell.Row, EndColumn = cell.Column });

            // Проверьте корректные значения
            string[] validValues = { "a", " ab", "cd ", " xyz " };
            foreach (string value in validValues)
            {
                cell.PutValue(value);
                Console.WriteLine($"Value: '{value}' - Valid: {cell.GetValidationValue()}");
            }

            // Проверьте некорректное значение
            string invalidValue = "toolong";
            cell.PutValue(invalidValue);
            Console.WriteLine($"Value: '{invalidValue}' - Valid: {cell.GetValidationValue()}");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


