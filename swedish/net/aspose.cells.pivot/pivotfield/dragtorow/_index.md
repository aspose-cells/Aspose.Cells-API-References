---
title: "PivotField.DragToRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om det angivna fältet kan dras till radregionen. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/dragtorow/
---
## PivotField.DragToRow property

Anger om det angivna fältet kan dras till radregionen. Standardvärdet är true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToRow { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.AllowDraggingToRow property. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Quarter";
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q3";
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;

            // Skapa pivottabell och hämta dess index
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta radfältet och sätt DragToRow-egenskapen
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToRow = true; // This allows the field to be dragged to row area

            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldDragToRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


