---
title: "Enum LookInType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LookInType enum. Representerar söktyp"
type: docs
url: /sv/net/aspose.cells/lookintype/
---
## LookInType enumeration

Representerar typen för look in.

```csharp
public enum LookInType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Formulas | `0` | Hittar det sökta objektet från formeln([`Formula`](../cell/formula/)) om cellen är en formel, annars hittas det från cellens ursprungliga värde (samma som OriginalValues). |
| Values | `1` | Hittar objektet från cellens ursprungliga värde([`Value`](../cell/value/)) och formaterade värde([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignorerar celler som är formel. För de celler som inte är formel är det samma som Values. |
| Comments | `3` | Hittar objektet endast från cellens kommentar. Ignorerar de celler som saknar kommentar. |
| OnlyFormulas | `4` | Ignorerar celler som inte är formel. För de celler som är formel hittas det sökta objektet från formeln([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Hitta objektet endast från cellens ursprungliga värde. |
| FormattedValues | `6` | Hitta objekt från cellens formaterade värde([`StringValue`](../cell/stringvalue/)) endast. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data och formler
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // Hitta cell som innehåller formeln med "B1"
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Skriv ut resultatet
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


