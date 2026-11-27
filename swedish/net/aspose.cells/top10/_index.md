---
title: "Klass Top10"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Top10-klass. Beskriv Top10‑villkorsformateringsregeln. Denna villkorsformateringsregel markerar celler vars värden faller inom de högsta N eller lägsta N‑intervallen som specificeras"
type: docs
url: /sv/net/aspose.cells/top10/
---
## Top10 class

Beskriv Top10-regeln för villkorsstyrd formatering. Denna villkorsstyrda formateringsregel markerar celler vars värden faller inom de översta N eller nedersta N intervallen, enligt specifikation.

```csharp
public class Top10
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Top10](top10/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Hämta eller ange om en \"top/bottom n\"‑regel är en \"bottom n\"‑regel. Standardvärdet är falskt. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Hämta eller ange om en \"top/bottom n\"‑regel är en \"top/bottom n percent\"‑regel. Standardvärdet är falskt. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Hämta eller ange värdet på \"n\" i en \"top/bottom n\"‑villkorsformateringsregel. Om IsPercent är sant måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Lägger till villkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Ställa in egenskaper
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Sparar Excel-filen
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


