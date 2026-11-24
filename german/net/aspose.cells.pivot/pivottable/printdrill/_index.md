---
title: "PivotTable.PrintDrill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt einen booleschen Wert an, der angibt, ob Drill-Indikatoren gedruckt werden sollen. Drucke Expand/Collapse-Schaltflächen, wenn sie in der Pivot-Tabelle angezeigt werden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/printdrill/
---
## PivotTable.PrintDrill property

Gibt einen booleschen Wert an, der angibt, ob Drill-Indikatoren gedruckt werden sollen. Druckt Expand-/Collapse‑Schaltflächen, wenn sie in der pivottable angezeigt werden.

```csharp
public bool PrintDrill { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintDrillDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Cars";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bikes";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 2500;

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demonstriere die PrintDrill-Eigenschaft
            pivotTable.PrintDrill = false; // Disable printing drill indicators
            pivotTable.ShowDrill = true;   // Show drill indicators on screen
            
            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePrintDrillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


