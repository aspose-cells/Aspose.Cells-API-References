---
title: "Slicer.Parent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer‑Eigenschaft. Gibt das Worksheet‑Objekt zurück, das diesen Slicer enthält. Nur lesbar"
type: docs
url: /de/net/aspose.cells.slicers/slicer/parent/
---
## Slicer.Parent property

Gibt das [`Worksheet`](../worksheet/)‑Objekt zurück, das diesen Slicer enthält. Nur lesbar.

```csharp
[Obsolete("Use Slicer.Worksheet property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Worksheet Parent { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die [`Worksheet`](../worksheet/)-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Januar 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyParentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";

            int tableIndex = sheet.ListObjects.Add("A1", "A4", true);
            ListObject table = sheet.ListObjects[tableIndex];

            int slicerIndex = sheet.Slicers.Add(table, 0, "B1");
            Slicer slicer = sheet.Slicers[slicerIndex];
            Worksheet currSheet = slicer.Parent;

            currSheet.Cells["C1"].Value = "ParentWorksheetAccessed";
            workbook.Save("SlicerParentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


