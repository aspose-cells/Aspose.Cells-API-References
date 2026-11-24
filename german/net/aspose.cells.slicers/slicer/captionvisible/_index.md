---
title: "Slicer.CaptionVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt zurück oder legt fest, ob die Kopfzeile, die die Slicer‑Beschriftung anzeigt, sichtbar ist. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells.slicers/slicer/captionvisible/
---
## Slicer.CaptionVisible property

Gibt zurück oder legt fest, ob die Kopfzeile, die die Slicer‑Beschriftung anzeigt, sichtbar ist. Der Standardwert ist true.

```csharp
[Obsolete("Use Slicer.ShowCaption property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool CaptionVisible { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [`ShowCaption`](../showcaption/)‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyCaptionVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Einen Slicer hinzufügen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Slicer-Eigenschaften festlegen, einschließlich CaptionVisible
            slicer.Caption = "Fruit Selection";
            slicer.CaptionVisible = true; // Show the caption header
            slicer.NumberOfColumns = 2;
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerCaptionVisibleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


