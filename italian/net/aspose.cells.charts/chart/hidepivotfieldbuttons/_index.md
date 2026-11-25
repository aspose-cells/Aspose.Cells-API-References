---
title: "Chart.HidePivotFieldButtons"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart"
type: docs
url: /it/net/aspose.cells.charts/chart/hidepivotfieldbuttons/
---
## Chart.HidePivotFieldButtons property

Indica se nascondere i pulsanti dei campi del grafico pivot solo quando il grafico è un PivotChart.

```csharp
public bool HidePivotFieldButtons { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Dimostra la proprietà HidePivotFieldButtons
            chart.HidePivotFieldButtons = false; // Show pivot field buttons
            chart.RefreshPivotData();

            // Salva la cartella di lavoro
            workbook.Save("HidePivotFieldButtonsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


