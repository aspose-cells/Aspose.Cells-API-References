---
title: "PivotField.DragToColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om det angivna fältet kan dras till kolumnregionen. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/dragtocolumn/
---
## PivotField.DragToColumn property

Anger om det angivna fältet kan dras till kolumnregionen. Standardvärdet är true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToColumn property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToColumn { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.AllowDraggingToColumn-egenskapen. Denna metod kommer att tas bort 12 månader senare, från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToColumnDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Item");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(8);

            // Lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hämta datafältet och sätt DragToColumn till true
            PivotField quantityField = pivotTable.DataFields[0];
            quantityField.DragToColumn = true; // This allows the field to be dragged to column area
            quantityField.DisplayName = "Total Quantity";

            // Beräkna data och spara
            pivotTable.CalculateData();
            workbook.Save("PivotFieldDragToColumnDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


