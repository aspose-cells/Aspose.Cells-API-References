---
title: "Range.ToHtml"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Konvertera området till HTML"
type: docs
url: /sv/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Konvertera området till HTML.

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Alternativ för att konvertera område till HTML. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite data i området A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Skapa ett område med fullt kvalificerat typnamn
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // Skapa HTML-sparalternativ
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Konvertera område till HTML
            byte[] htmlData = range.ToHtml(options);
            
            // Spara HTML till fil
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


