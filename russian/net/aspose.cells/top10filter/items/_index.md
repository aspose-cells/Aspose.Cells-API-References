---
title: "Top10Filter.Items"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Top10Filter. Получает и задаёт верхнее или нижнее значение, используемое в качестве критерия фильтра"
type: docs
url: /ru/net/aspose.cells/top10filter/items/
---
## Top10Filter.Items property

Получает и задает верхнее или нижнее значение, используемое в качестве критерия фильтра.

```csharp
public int Items { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyItemsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grapes");
            worksheet.Cells["A6"].PutValue("Mango");
            
            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Применить фильтр top 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Получить фильтр и продемонстрировать свойство Items
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            int itemsCount = filter.GetTop10Value().Items;
            
            Console.WriteLine("Top 10 Filter Items Count: " + itemsCount);
        }
    }
}
```

### См. также

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


