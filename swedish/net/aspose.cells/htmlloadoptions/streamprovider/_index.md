---
title: "HtmlLoadOptions.StreamProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions‑egenskap. Hämtar eller anger StreamProviderImportHtmlFile för import av objekt"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Hämtar eller anger StreamProviderImportHtmlFile för att importera objekt.

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
    public class HtmlLoadOptionsPropertyStreamProviderDemo : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            // Initiera ström vid behov
        }

        public Stream ProvideStream(StreamProviderOptions options)
        {
            // Returnera en ström för läsning/skrivning
            return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Stäng strömmen
            options.Stream.Close();
        }

        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");

            // Spara med anpassad StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            workbook.Save("output.html", saveOptions);

            // Ladda med anpassad StreamProvider
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("output.html", loadOptions);

            // Verifiera inläst data
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Se även

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


