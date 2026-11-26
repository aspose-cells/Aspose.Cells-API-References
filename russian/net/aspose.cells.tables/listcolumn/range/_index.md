---
title: "ListColumn.Range"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListColumn. Получает диапазон этого столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Получает диапазон этого столбца списка.

```csharp
public Range Range { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для создания объекта списка
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Создать объект списка
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // Получить первый столбец списка
            ListColumn listCol = listObj.ListColumns[0];
            
            // Получить доступ к диапазону столбца списка
            Aspose.Cells.Range range = listCol.Range;
            
            // Отобразить информацию о диапазоне
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Изменить ячейки в диапазоне
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Сохраните книгу
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


