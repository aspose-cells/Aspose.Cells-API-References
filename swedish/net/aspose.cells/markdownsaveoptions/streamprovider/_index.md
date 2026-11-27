---
title: "MarkdownSaveOptions.StreamProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions-egenskap. Hämtar eller anger IStreamProvider för export av objekt. Om null sparas de exporterade objekten i samma katalog som utdatafilen"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Hämtar eller anger IStreamProvider för export av objekt. Om `null` sparas de exporterade objekten i samma katalog som utdatafilen.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MarkdownSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Hello";
            worksheet.Cells["B1"].Value = "World";

            try
            {
                // Skapa en instans av MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visa det aktuella StreamProvider-värdet (null som standard)
                Console.WriteLine("Current StreamProvider: " + (saveOptions.StreamProvider == null ? "null" : "set"));

                // Skapa en anpassad StreamProvider-implementation
                CustomStreamProvider streamProvider = new CustomStreamProvider();
                saveOptions.StreamProvider = streamProvider;

                // Visa det uppdaterade StreamProvider-värdet
                Console.WriteLine("Updated StreamProvider: " + (saveOptions.StreamProvider != null ? "set" : "null"));

                // Spara arbetsboken med den anpassade StreamProvider
                workbook.Save("StreamProviderDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved with custom StreamProvider.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    // Anpassad implementation av IStreamProvider
    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            Console.WriteLine("Initializing stream");
        }

        public void CloseStream(StreamProviderOptions options)
        {
            Console.WriteLine("Closing stream");
        }
    }
}
```

### Se även

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


