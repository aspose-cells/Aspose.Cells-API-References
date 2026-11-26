---
title: "SlicerCacheItemCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SlicerCacheItemCollection. Получает объект SlicerCacheItem по индексу"
type: docs
url: /ru/net/aspose.cells.slicers/slicercacheitemcollection/item/
---
## SlicerCacheItemCollection indexer

Получает объект SlicerCacheItem по индексу.

```csharp
public SlicerCacheItem this[int index] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу и добавить сводную таблицу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить срез
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = slicers[slicerIndex];
            
            // Получить доступ к элементам кэша срезов с помощью свойства Item
            SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
            if (items.Count > 0)
            {
                SlicerCacheItem item = items[0]; // Demonstrating Item property usage
                Console.WriteLine("First slicer item: " + item.Value);
            }
        }
    }
}
```

### См. также

* class [SlicerCacheItem](../../slicercacheitem/)
* class [SlicerCacheItemCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


