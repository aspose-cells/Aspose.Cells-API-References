---
title: "Validation.RemoveArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Удалить настройки проверки в диапазоне"
type: docs
url: /ru/net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

Удалить настройки проверки в диапазоне.

```csharp
public void RemoveArea(CellArea cellArea)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellArea | CellArea | области, где эти настройки проверки должны быть удалены. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку на листе
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Добавить начальную область проверки
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            validation.AddArea(initialArea);

            // Добавить другую область к проверке
            CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
            validation.AddArea(additionalArea);

            Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);

            // Удалить дополнительную область
            validation.RemoveArea(additionalArea);

            Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);

            // Добавить несколько областей
            CellArea[] multipleAreas = new CellArea[]
            {
                CellArea.CreateCellArea(2, 2, 2, 2),
                CellArea.CreateCellArea(3, 3, 3, 3),
                CellArea.CreateCellArea(4, 4, 4, 4)
            };
            validation.AddAreas(multipleAreas, false, false);

            Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);

            // Удалить одну из областей
            validation.RemoveArea(multipleAreas[1]);

            Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


