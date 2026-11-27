---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Anger hur OfficeMath‑objekt exporteras till Markdown. Standardvärdet är Image."
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

Anger hur OfficeMath-objekt exporteras till Markdown. Standardvärdet är Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata inklusive en formel som kan innehålla OfficeMath
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Skapa Markdown‑sparalternativ
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visa det aktuella värdet för OfficeMathOutputType
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // Ställ in OfficeMathOutputType till MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Spara arbetsboken med MathML‑utmatningstyp
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Byt till Image‑utmatningstyp
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Spara arbetsboken med Image‑utmatningstyp
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


