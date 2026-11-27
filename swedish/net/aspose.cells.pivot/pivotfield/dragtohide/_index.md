---
title: "PivotField.DragToHide"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om detta pivottfält kan tas bort från PivotTable-vyn. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/dragtohide/
---
## PivotField.DragToHide property

Anger om detta pivotfält kan tas bort från pivottabellvyn. Standardvärdet är true.

```csharp
[Obsolete("Use PivotField.AllowRemovingFromView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToHide { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.AllowRemovingFromView egenskap. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToHideDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;
            cells["B5"].Value = 250;

            // Skapa pivottabell - Hämta indexet först, sedan hämta PivotTable-objektet
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält och konfigurera DragToHide
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.DragToHide = true; // Core demonstration of the property
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldDragToHideDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


