---
title: "ValidationCollection.RemoveACell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ValidationCollection. Удаляет все настройки проверки в ячейке"
type: docs
url: /ru/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Удаляет все настройки проверок в ячейке.

```csharp
public void RemoveACell(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки. |
| column | Int32 | Индекс столбца ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить проверку в ячейку A1 (строка 0, столбец 0)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // Удалить проверку из ячейки A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### См. также

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


