---
title: "HtmlSaveOptions.PresentationPreference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om HTML‑ eller MHT‑fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Anger om HTML- eller MHT-fil föredras för presentation. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true.

```csharp
public bool PresentationPreference { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Presentation Preference Test");
            worksheet.Cells["B1"].PutValue(123.45);
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // Ställ in HTML‑sparalternativ med PresentationPreference
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = false;

            // Spara till minnesström för demonstration
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                Console.WriteLine("Workbook saved with PresentationPreference=true");
            }
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


