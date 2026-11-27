---
title: "PivotField.DragToPage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om det angivna fältet kan dras till sidregionen. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/dragtopage/
---
## PivotField.DragToPage property

Anger om det angivna fältet kan dras till sidområdet. Standardvärdet är true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToPage { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd i stället PivotField.AllowDraggingToPage property. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToPageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Cars";
            cells["A4"].Value = "Bikes";
            cells["A5"].Value = "Cars";
            
            cells["B1"].Value = "Region";
            cells["B2"].Value = "North";
            cells["B3"].Value = "South";
            cells["B4"].Value = "North";
            cells["B5"].Value = "South";
            
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till fält och konfigurera DragToPage
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField regionField = pivotTable.PageFields[fieldIndex];
            
            // Demonstrera DragToPage-egenskapen
            regionField.DragToPage = false; // Disable dragging to page area
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsbok
            workbook.Save("PivotFieldDragToPageDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


