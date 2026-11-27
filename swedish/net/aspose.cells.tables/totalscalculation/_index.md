---
title: "Enum TotalsCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TotalsCalculation enum. Bestämmer typen av beräkning i totalsraden för listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Bestämmer beräkningstypen i totalsraden för listkolumnen.

```csharp
public enum TotalsCalculation
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Sum | `6` | Representerar Sum totals-beräkning. |
| Count | `2` | Representerar Count totals-beräkning. |
| Average | `1` | Representerar Average totals-beräkning. |
| Max | `4` | Representerar Max totals-beräkning. |
| Min | `5` | Representerar Min totals-beräkning. |
| Var | `8` | Representerar Var totals-beräkning. |
| CountNums | `3` | Representerar Count Nums totals-beräkning. |
| StdDev | `7` | Representerar StdDev totals-beräkning. |
| None | `0` | Representerar No totals-beräkning. |
| Custom | `9` | Representerar anpassad beräkning. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

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

            // Lägg till en tabell i kalkylbladet
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Visa totalsrad
            table.ShowTotals = true;

            // Åtkomst till den femte kolumnen i tabellen
            ListColumn listColumn = table.ListColumns[4];

            // Ställ in TotalsCalculation egenskapen till Sum
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // Eventuellt, ange en formel för kolumnen
            listColumn.Formula = "=[A]";

            // Spara arbetsboken
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


