---
title: "SlicerCache.List"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SlicerCache-Eigenschaft. Gibt an, ob der mit dem angegebenen Slicer-Cache verbundene Slicer auf einer NonOLAP-Datenquelle basiert"
type: docs
url: /de/net/aspose.cells.slicers/slicercache/list/
---
## SlicerCache.List property

Gibt an, ob der mit dem angegebenen Slicer-Cache verbundene Slicer auf einer Nicht-OLAP-Datenquelle basiert.

```csharp
public bool List { get; }
```

### Beispiele

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

            // Erstelle Beispieldaten
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Tabelle mit korrekter Überladung erstellen
            int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Füge Slicer hinzu
            int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
            Slicer slicer = sheet.Slicers[slicerIdx];

            // Auf Slicer-Cache zugreifen
            SlicerCache cache = slicer.SlicerCache;

            // Verwendung der List-Eigenschaft demonstrieren
            Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
        }
    }
}
```

### Siehe auch

* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


