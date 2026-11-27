---
title: "PivotTable.RowRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Returnerar ett CellArea-objekt som representerar det område som innehåller radområdet i pivottabellrapporten. Endast läsning."
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Returnerar ett CellArea-objekt som representerar det område som innehåller radområdet i PivotTable‑rapporten. Endast läsning.

```csharp
public CellArea RowRange { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Uppdatera alla pivottabeller i arbetsboken
            workbook.Worksheets.RefreshAll();
            
            // Hämta den första pivottabellen från det första kalkylbladet
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Hämta radområdet för pivottabellen
            CellArea rowRange = pivotTable.RowRange;
            
            // Visa radområdets koordinater
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Hämta kolumnområdet för pivottabellen
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Visa kolumnområdets koordinater
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


