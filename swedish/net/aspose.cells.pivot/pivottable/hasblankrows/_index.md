---
title: "PivotTable.HasBlankRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om tomma rader ska läggas till. Denna egenskap gäller endast för PivotTable-autoformattyper som behöver lägga till tomma rader"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Anger om tomma rader ska läggas till. Denna egenskap gäller endast för PivotTable-autoformattyper som behöver lägga till tomma rader.

```csharp
[Obsolete("Use PivotField.InsertBlankRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBlankRows { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.InsertBlankRow-egenskapen. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyHasBlankRowsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet dataSheet = wb.Worksheets[0];
            
            // Skapa exempeldata
            dataSheet.Cells[0, 0].PutValue("Category");
            dataSheet.Cells[0, 1].PutValue("Product");
            dataSheet.Cells[0, 2].PutValue("Sales");
            
            Random rnd = new Random();
            for (int i = 1; i <= 10; i++)
            {
                dataSheet.Cells[i, 0].PutValue(rnd.Next(2) == 0 ? "Electronics" : "Furniture");
                dataSheet.Cells[i, 1].PutValue("Product " + rnd.Next(1, 4));
                dataSheet.Cells[i, 2].PutValue(rnd.Next(100, 1000));
            }

            // Lägg till pivottabell
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Sheet1!A1:C11", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Demonstrera HasBlankRows-egenskapen
            pivotTable.HasBlankRows = false; // Remove blank lines between items
            
            // Spara arbetsboken
            wb.Save("PivotTableHasBlankRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


