---
title: "Worksheet.Slicers"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Slicer‑Sammlung im Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Rufen Sie die Slicer‑Sammlung im Arbeitsblatt ab.

```csharp
public SlicerCollection Slicers { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySlicersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Eine Tabelle hinzufügen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Slicer zum Arbeitsblatt hinzufügen
            worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
            worksheet.Slicers.Add(table, 1, "D1");
            worksheet.Slicers.Add(table, table.ListColumns[0], "G1");

            // Speichere die Arbeitsmappe
            workbook.Save("SlicersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


