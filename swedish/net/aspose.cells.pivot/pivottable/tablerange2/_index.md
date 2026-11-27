---
title: "PivotTable.TableRange2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Returnerar ett CellArea‑objekt som representerar området som innehåller hela pivottabellsrapporten inklusive sidfält. Skrivskyddad"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Returnerar ett CellArea-objekt som representerar intervallet som innehåller hela PivotTable-rapporten, inklusive sidfält. Endast läsning.

```csharp
public CellArea TableRange2 { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange2Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Hämta TableRange2 som inkluderar hela pivottabellen
            CellArea tableRange2 = pivotTable.TableRange2;
            Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
                $"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");

            // Skapa ett område baserat på TableRange2
            Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
                tableRange2.StartRow, 
                tableRange2.StartColumn, 
                tableRange2.EndRow - tableRange2.StartRow + 1, 
                tableRange2.EndColumn - tableRange2.StartColumn + 1);

            // Skriv ut områdesadressen
            Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


