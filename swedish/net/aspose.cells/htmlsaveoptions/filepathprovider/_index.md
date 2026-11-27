---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar eller anger IFilePathProvider för att exportera Worksheet till html separat"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Hämtar eller anger IFilePathProvider för separat export av kalkylblad till html.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Skapa HtmlSaveOptions och ange FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // Spara arbetsboken i HTML-format
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Anpassad logik för att generera filsökvägar
            return $"custom_{sheetName}";
        }
    }
}
```

### Se även

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


