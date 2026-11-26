---
title: "SlicerCache.List"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SlicerCache. Указывает, основан ли срез, связанный с указанным кэшем срезов, на источнике данных NonOLAP"
type: docs
url: /ru/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

Указывает, основан ли slicer, связанный с указанным кэшем slicer, на источнике данных Non-OLAP.

```csharp
public bool List { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCachePropertyListDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Создать таблицу с правильной перегрузкой
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Добавить срез
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // Получить доступ к кэшу срезов
            SlicerCache cache = slicer.SlicerCache;

            // Продемонстрировать использование свойства List
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### См. также

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


