---
title: "Chart.HidePivotFieldButtons"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Gibt an, ob die Pivot-Diagramm-Feldschaltflächen nur ausgeblendet werden, wenn das Diagramm ein PivotChart ist."
type: docs
url: /de/net/aspose.cells.charts/chart/hidepivotfieldbuttons/
---
## Chart.HidePivotFieldButtons property

Gibt an, ob die Pivot‑Diagramm‑Feldschaltflächen nur ausgeblendet werden sollen, wenn das Diagramm ein PivotChart ist.

```csharp
public bool HidePivotFieldButtons { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ChartPropertyHidePivotFieldButtonsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
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

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Demonstration der HidePivotFieldButtons-Eigenschaft
            chart.HidePivotFieldButtons = false; // Show pivot field buttons
            chart.RefreshPivotData();

            // Speichere die Arbeitsmappe
            workbook.Save("HidePivotFieldButtonsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


