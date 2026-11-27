---
title: "Struktur CellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellArea struct. Representerar ett område av celler"
type: docs
url: /sv/net/aspose.cells/cellarea/
---
## CellArea structure

Representerar ett område av celler.

```csharp
public struct CellArea : IComparable
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Skapar ett cellområde. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Skapar ett cellområde. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Jämför två CellArea-objekt enligt deras övre vänstra hörn. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Returnerar en sträng som representerar det aktuella cellområdeobjektet. |

## Fält

| Namn | Beskrivning |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Hämtar eller anger slutkolumnen för detta område. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Hämtar eller anger slutraden för detta område. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Hämtar eller anger startkolumnen för detta område. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Hämtar eller anger startraden för detta område. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Skapa cellområde
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Lägg till en villkorlig formateringsregel i kalkylbladet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Spara arbetsboken
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // Demonstrera ToString-metoden
            Console.WriteLine(ca.ToString());

            // Demonstrera CompareTo-metoden
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


