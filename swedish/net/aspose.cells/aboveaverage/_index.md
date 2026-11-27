---
title: "Klass AboveAverage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AboveAverage-klass. Beskriver AboveAverage-regeln för villkorsstyrd formatering. Denna regel markerar celler som är över eller under genomsnittet för alla värden i området"
type: docs
url: /sv/net/aspose.cells/aboveaverage/
---
## AboveAverage class

Beskriv regeln för villkorsformatering AboveAverage. Denna villkorsformateringsregel markerar celler som är över eller under genomsnittet för alla värden i intervallet.

```csharp
public class AboveAverage
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [AboveAverage](aboveaverage/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Hämta eller ange flaggan som indikerar om regeln är en \"above average\"-regel. 'true' betyder 'above average'. Standardvärdet är true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Hämta eller ange flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva genomsnittet, eller exkluderar det värdet. 'true' betyder att genomsnittsvärdet inkluderas i kriterierna. Standardvärdet är false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Hämta eller ange antalet standardavvikelser som ska inkluderas över eller under genomsnittet i regeln för villkorsstyrd formatering. Inmatningsvärdet måste vara mellan 0 och 3 (inklusive 0 och 3). Att sätta värdet till 0 betyder att stdDev inte är angivet. Standardvärdet är 0. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Lägg till en samling för villkorsstyrd formatering i kalkylbladet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Definiera cellområdet där den villkorsstyrda formateringen ska tillämpas
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Lägg till ett above average-villkor i samlingen
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Ange bakgrundsfärgen för villkoret
            fc.Style.BackgroundColor = Color.Yellow;

            // Ange egenskaper för above average-villkoret
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Spara arbetsboken
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


