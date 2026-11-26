---
title: "FindOptions.SetRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FindOptions. Устанавливает диапазон поиска"
type: docs
url: /ru/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Задает диапазон поиска.

```csharp
public void SetRange(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | искомый диапазон. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // Создайте FindOptions и установите диапазон поиска
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // Поиск в указанном диапазоне
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


