---
title: "HtmlSaveOptions.StreamProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Hämtar eller anger IStreamProvider för export av objekt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Hämtar eller anger IStreamProvider för export av objekt.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Skapa en temporär katalog för utdata
            string outputDir = Path.Combine(Path.GetTempPath(), "AsposeStreamProviderDemo");
            Directory.CreateDirectory(outputDir);

            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("StreamProvider Demo");

            // Konfigurera HTML-sparalternativ med anpassad stream provider
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.StreamProvider = new ExportStreamProvider(outputDir);

            // Spara arbetsboken som HTML
            string outputPath = Path.Combine(outputDir, "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine($"File saved with StreamProvider to: {outputPath}");
        }
    }

    public class ExportStreamProvider : IStreamProvider
    {
        private readonly string _outputDirectory;

        public ExportStreamProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // Initiering om behövs
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            string filePath = Path.Combine(_outputDirectory, options.CustomPath);
            return new FileStream(filePath, FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementering enligt gränssnittet
        }
    }
}
```

### Se även

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


