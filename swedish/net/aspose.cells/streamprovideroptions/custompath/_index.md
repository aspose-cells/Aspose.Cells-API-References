---
title: "StreamProviderOptions.CustomPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StreamProviderOptions-egenskap. Den anpassade sökvägs‑URL:en som användaren anger sparas i den genererade HTML-filen för den refererade källan. Om den inte definieras av användaren används DefaultPath. Till exempel kommer bladdata att sparas av användaren till d/sheet001.htm; URL:en som används i huvud‑HTML‑filen bör vara d/sheet001.htm eller någon annan giltig relativ sökväg som kan nås av huvud‑HTML‑filen."
type: docs
url: /sv/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

Den anpassade sökvägen (URL) som användaren sparar i den genererade html-filen för den refererade källan. Om den inte definieras av användaren används DefaultPath. Till exempel kommer bladdata att sparas av användaren till d:/sheet001.htm, URL:en som används i huvud‑html‑filen bör vara "d:/sheet001.htm" eller någon annan giltig relativ sökväg som kan nås av huvud‑html‑filen.

```csharp
public string CustomPath { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Ställ in HTML‑sparalternativ med anpassad strömleverantör
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // Skapa anpassad strömleverantör med CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Spara arbetsboken
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Verifiera att den anpassade sökvägen användes
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Förenklad implementation av anpassad strömleverantör
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Implementering skulle placeras här
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementering skulle placeras här
        }
    }
}
```

### Se även

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


