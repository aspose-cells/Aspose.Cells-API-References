---
title: "Enum AutoFitWrappedTextType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AutoFitWrappedTextType enum. Representerar typen av automatiskt anpassad radbrytningstext"
type: docs
url: /sv/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Representerar typen av automatisk anpassning av radbrytning i text.

```csharp
public enum AutoFitWrappedTextType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Fungerar som MS Excel. |
| Paragraph | `1` | Anpassa bredd automatiskt med det längsta stycket. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // Skapa ett område A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Sammanfoga cellerna
            range.Merge();

            // Skapa ett område A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Sammanfoga cellerna
            range2.Merge();

            // Skapa AutoFitterOptions och ange AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Auto‑anpassa rader med de angivna alternativen
            worksheet.AutoFitRows(options);

            // Spara arbetsboken
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


