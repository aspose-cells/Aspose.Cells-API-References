---
title: "PivotTable.ColumnRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Returnerar ett CellArea-objekt som representerar det område som innehåller kolumnområdet i PivotTable-rapporten. Endast läs"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/columnrange/
---
## PivotTable.ColumnRange property

Returnerar ett CellArea‑objekt som representerar det område som innehåller kolumnområdet i pivottabellsrapporten. Endast läsning.

```csharp
public CellArea ColumnRange { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnRangeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;
            
            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Hämta kolumnområdet för pivottabellen
            CellArea columnRange = pivotTable.ColumnRange;
            Console.WriteLine("Pivot Table Column Range: " + columnRange);
            
            // Spara arbetsboken
            workbook.Save("PivotTableColumnRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


