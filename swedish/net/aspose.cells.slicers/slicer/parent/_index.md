---
title: "Slicer.Parent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Returnerar Worksheet‑objektet som innehåller den här slicern. Läs‑endast"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/parent/
---
## Slicer.Parent property

Returnerar [`Worksheet`](../worksheet/)‑objektet som innehåller den här slicern. Läs‑endast.

```csharp
[Obsolete("Use Slicer.Worksheet property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Worksheet Parent { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället [`Worksheet`](../worksheet/)‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med januari 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


