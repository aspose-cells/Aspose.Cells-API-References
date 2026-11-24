---
title: "Slicer.Placement"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer‑Eigenschaft. Gibt an, wie das Zeichenobjekt an den darunterliegenden Zellen befestigt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt."
type: docs
url: /de/net/aspose.cells.slicers/slicer/placement/
---
## Slicer.Placement property

Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die Eigenschaft steuert die Platzierung eines Objekts auf einem Arbeitsblatt.

```csharp
[Obsolete("Use Shape.Placement property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PlacementType Placement { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die [`Placement`](../../../aspose.cells.drawing/shape/placement/)-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Januar 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyPlacementDemo
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
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Füge einen Slicer für die Pivot‑Tabelle hinzu
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Setze Slicer‑Eigenschaften einschließlich Placement
            slicer.Title = "Fruit Slicer";
            slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
            slicer.HeightPixel = 200;
            slicer.WidthPixel = 150;

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerPlacementDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


