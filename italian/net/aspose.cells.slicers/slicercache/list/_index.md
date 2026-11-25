---
title: "SlicerCache.List"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SlicerCache. Indica se lo slicer associato alla cache slicer specificata è basato su una fonte dati NonOLAP"
type: docs
url: /it/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

Indica se lo slicer associato alla cache dello slicer specificata è basato su una fonte dati non OLAP.

```csharp
public bool List { get; }
```

### Esempi

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

            // Crea dati di esempio
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Crea una tabella con overload corretto
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Aggiungi slicer
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // Accedi alla cache slicer
            SlicerCache cache = slicer.SlicerCache;

            // Dimostra l'uso della proprietà List
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### Vedi anche

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


