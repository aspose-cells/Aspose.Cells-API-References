---
title: "Gränssnitt IStreamProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IStreamProvider-gränssnitt. Representerar den exporterade strömleverantören"
type: docs
url: /sv/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Representerar leverantören av den exporterade strömmen.

```csharp
public interface IStreamProvider
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Stänger strömmen. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Hämtar strömmen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // Implementering av InitStream-metoden
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // Implementering av CloseStream-metoden
        public void CloseStream(StreamProviderOptions options)
        {
            // Stäng strömmen om den inte är null
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange viss data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello World");

            // Skapa HtmlSaveOptions och ange StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Spara arbetsboken i HTML-format
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Läs in arbetsboken från HTML-format
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Visa den inlästa datan
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


