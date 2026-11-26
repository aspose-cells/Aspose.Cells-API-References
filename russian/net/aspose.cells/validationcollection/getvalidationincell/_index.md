---
title: "ValidationCollection.GetValidationInCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ValidationCollection. Возвращает проверку, примененную к указанной ячейке"
type: docs
url: /ru/net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Получает проверку, применённую к указанной ячейке.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Возвращает объект [`Validation`](../../validation/) или null, если для указанной ячейки нет проверки

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку данных в ячейку A1 (0,0)
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "\"Option1,Option2,Option3\"";
            
            // Создать CellArea с параметрами StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Получить проверку из ячейки A1 (0,0)
            Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
            
            if (validationInCell != null && validationInCell.Type == ValidationType.List)
            {
                Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
            }
        }
    }
}
```

### См. также

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


