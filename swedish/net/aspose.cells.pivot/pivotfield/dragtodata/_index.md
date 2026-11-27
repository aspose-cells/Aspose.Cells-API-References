---
title: "PivotField.DragToData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField‑egenskap. Anger om det angivna fältet kan dras till värdeområdet. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/dragtodata/
---
## PivotField.DragToData property

Anger om det angivna fältet kan dras till värdeområdet. Standardvärdet är true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToData { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.AllowDraggingToData egenskap. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Bikes";
            cells["A4"].Value = "Cars";
            cells["A5"].Value = "Cars";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 1500;
            cells["C4"].Value = 2000;
            cells["C5"].Value = 2500;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält och konfigurera DragToData
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];
            rowField.DragToData = true; // Allow dragging this field to data area
            
            // Lägg till kolumnfält
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldDragToDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


