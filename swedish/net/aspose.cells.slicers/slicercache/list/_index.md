---
title: "SlicerCache.List"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SlicerCache-egenskap. Anger om slicern som är kopplad till den angivna slicer-cachen är baserad på en NonOLAP-datakälla"
type: docs
url: /sv/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

Indikerar om skärmningskontrollen som är associerad med den angivna skärmningscachen är baserad på en icke‑OLAP-datakälla.

```csharp
public bool List { get; }
```

### Exempel

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

            // Skapa exempeldata
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Skapa tabell med korrekt överlagring
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Lägg till skärmningskontrollen
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // Åtkomst till slicer-cache
            SlicerCache cache = slicer.SlicerCache;

            // Demonstrera användning av List-egenskapen
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### Se även

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


