---
title: "Worksheet.Validations"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию настроек проверки данных в листе"
type: docs
url: /ru/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Получает коллекцию настроек проверки данных в листе.

```csharp
public ValidationCollection Validations { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку данных в ячейку A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Исправление: создать CellArea с параметрами StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Получить проверку данных из ячейки A1
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Вывести тип валидации
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Сохраните книгу
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### См. также

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


