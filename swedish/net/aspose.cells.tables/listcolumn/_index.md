---
title: "Klass ListColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.ListColumn-klass. Representerar en kolumn i en tabell"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Representerar en kolumn i en tabell.

```csharp
public class ListColumn
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Hämtar och anger formeln för listkolumnen. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Indikerar om formeln är en matrisformel. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Hämtar och anger namnet på kolumnen. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Hämtar intervallet för denna listkolumn. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Hämtar och anger typen av beräkning i totalsraden för listkolumnen. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Hämtar och anger visningsetiketterna för totalsraden. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Hämtar formeln för denna listkolumn. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Hämtar formeln för totalsraden för denna listkolumn. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Hämtar stilen för data i denna kolumn i tabellen. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Ställer in formeln för denna listkolumn. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Hämtar formeln för totalsraden för denna listkolumn. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Ställer in stilen för data i denna kolumn i tabellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i arbetsbladet med några data
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Lägg till ett ListObject (tabell) i kalkylbladet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Åtkomst till ListColumn och ange dess egenskaper
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Spara arbetsboken
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


