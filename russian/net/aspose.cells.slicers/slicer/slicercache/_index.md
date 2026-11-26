---
title: "Slicer.SlicerCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает объект SlicerCache, связанный с срезом. Только для чтения."
type: docs
url: /ru/net/aspose.cells.slicers/slicer/slicercache/
---
## Slicer.SlicerCache property

Возвращает объект SlicerCache, связанный с слайсером. Только для чтения.

```csharp
public SlicerCache SlicerCache { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertySlicerCacheDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Создать таблицу из диапазона данных
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Добавить сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Добавить слайсер
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Продемонстрировать использование SlicerCache
            SlicerCache slicerCache = slicer.SlicerCache;
            Console.WriteLine("Slicer Cache Name: " + slicerCache.Name);
            Console.WriteLine("Slicer Cache Source Name: " + slicerCache.SourceName);
            Console.WriteLine("Slicer Cache Items Count: " + slicerCache.SlicerCacheItems.Count);

            // Сохраните книгу
            workbook.Save("SlicerCacheDemo.xlsx");
        }
    }
}
```

### См. также

* class [SlicerCache](../../slicercache/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


