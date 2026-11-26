---
title: "SlicerCacheItem.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SlicerCacheItem. Возвращает текст метки для элемента среза"
type: docs
url: /ru/net/aspose.cells.slicers/slicercacheitem/value/
---
## SlicerCacheItem.Value property

Возвращает текст метки для элемента slicer.

```csharp
public string Value { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertyValueDemo
    {
        public static void Run()
        {
            // Создать книгу с образцовыми данными
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Создать примерные данные для сводной таблицы
            ws.Cells["A1"].PutValue("Name");
            ws.Cells["A2"].PutValue("Alex");
            ws.Cells["A3"].PutValue("Sam");
            ws.Cells["A4"].PutValue("Alex");
            ws.Cells["A5"].PutValue("John");
            
            // Создать сводную таблицу
            int index = ws.PivotTables.Add("A1:A5", "E1", "PivotTable1");
            PivotTable pt = ws.PivotTables[index];
            pt.AddFieldToArea(PivotFieldType.Row, "Name");
            
            // Добавить срез
            int slicerIndex = ws.Slicers.Add(pt, "Name", "Slicer1");
            Slicer slicer = ws.Slicers[slicerIndex];
            
            // Продемонстрировать использование свойства Value
            Console.WriteLine("All items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                Console.WriteLine(item.Value);
            }
            
            // Выбрать только "Alex"
            Console.WriteLine("\nSelecting only Alex:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = (item.Value == "Alex");
            }
            slicer.Refresh();
            
            // Показать выбранные элементы
            Console.WriteLine("\nSelected items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                if (item.Selected)
                {
                    Console.WriteLine(item.Value);
                }
            }
            
            // Выбрать все элементы
            Console.WriteLine("\nSelecting all items:");
            foreach (SlicerCacheItem item in slicer.SlicerCache.SlicerCacheItems)
            {
                item.Selected = true;
            }
            slicer.Refresh();
        }
    }
}
```

### См. также

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


