---
title: "Slicer.ColumnWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt die Breite jeder Spalte im Slicer in Punkten zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.slicers/slicer/columnwidth/
---
## Slicer.ColumnWidth property

Gibt die Breite jeder Spalte im Slicer zurück oder legt sie fest, in der Einheit Punkte.

```csharp
public double ColumnWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            
            // PivotTable hinzufügen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Füge Slicer hinzu
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Spaltenbreite in Punkten festlegen
            slicer.ColumnWidth = 80;
            
            // Speichere die Arbeitsmappe
            workbook.Save("SlicerColumnWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


