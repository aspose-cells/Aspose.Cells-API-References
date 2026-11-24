---
title: "Slicer.AlternativeText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt die beschreibende alternative Textzeichenfolge des Slicer-Objekts zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.slicers/slicer/alternativetext/
---
## Slicer.AlternativeText property

Gibt die beschreibende (alternative) Textzeichenfolge des Slicer-Objekts zurück oder legt sie fest.

```csharp
[Obsolete("Use Shape.AlternativeText property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AlternativeText { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [`AlternativeText`](../../../aspose.cells.drawing/shape/alternativetext/) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1:A3", "", true)];
            table.DisplayName = "Table1";

            int slicerIndex = worksheet.Slicers.Add(table, 0, "C1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.AlternativeText = "AlternativeText test";

            workbook.Save("SlicerAlternativeTextDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


