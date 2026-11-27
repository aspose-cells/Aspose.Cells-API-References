---
title: "Enum TextAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TextAlignmentType enum. Enumererar textjusteringstyper"
type: docs
url: /sv/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Enumererar typer av textjustering.

```csharp
public enum TextAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| General | `1792` | Representerar allmän textjustering. |
| Bottom | `528` | Representerar nedre textjustering. |
| Center | `1802` | Representerar centrerad textjustering. |
| CenterAcross | `1286` | Representerar centrerad över textjustering. |
| Distributed | `807` | Representerar distribuerad textjustering. |
| Fill | `1284` | Representerar fyllningstextjustering. |
| Justify | `1821` | Representerar justifierad textjustering. |
| Left | `257` | Representerar vänsterjustering av text. |
| Right | `259` | Representerar högerjustering av text. |
| Top | `512` | Representerar toppjustering av text. |
| JustifiedLow | `832` | Justerar texten med en justerad kashidalängd för arabisk text. |
| ThaiDistributed | `896` | Distribuerar thailändsk text på ett speciellt sätt, eftersom varje tecken behandlas som ett ord. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Lägg till en kommentar till en cell
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Anpassa diagrammets titel
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Spara arbetsboken
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Skriv ut resultaten
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


