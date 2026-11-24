---
title: "Slicer.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt die Breite des angegebenen Slicers in Punkten zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.slicers/slicer/width/
---
## Slicer.Width property

Gibt die Breite des angegebenen Slicers zurück oder legt sie fest, in Punkten.

```csharp
[Obsolete("Use Shape.WidthPt property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double Width { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.WidthPt. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthDemo
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
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Einen Slicer hinzufügen
            int slicerIndex = worksheet.Slicers.Add(pivotTable, 0, 0, "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Richtige Methode, um eine Pivot-Verbindung zum Slicer hinzuzufügen
            slicer.AddPivotConnection(pivotTable);

            // Slicer-Eigenschaften einschließlich Breite festlegen
            slicer.Caption = "Fruit Selection";
            slicer.Width = 150; // Setting the width in points
            slicer.Height = 200;

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


