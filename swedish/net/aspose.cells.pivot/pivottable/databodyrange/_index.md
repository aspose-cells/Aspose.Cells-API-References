---
title: "PivotTable.DataBodyRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Returnerar ett CellArea‑objekt som representerar det område som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. Skrivskyddad"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Returnerar ett [`CellArea`](../../../aspose.cells/cellarea/)‑objekt som representerar det område som innehåller dataområdet i listan mellan rubrikraden och infogningsraden. Skrivskyddad.

```csharp
public CellArea DataBodyRange { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Lägg till exempeldata för pivottabell
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Lägg till pivottabell
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabell
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Uppdatera pivot‑tabellens data
            pivot.RefreshData();
            pivot.CalculateData();

            // Demonstrera användning av DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Spara arbetsboken
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


