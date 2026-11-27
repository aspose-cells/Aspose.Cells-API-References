---
title: "Gränssnitt IFilePathProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IFilePathProvider-gränssnitt. Representerar leverantören av den exporterade filsökvägen"
type: docs
url: /sv/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Representerar leverantören av den exporterade filsökvägen.

```csharp
public interface IFilePathProvider
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Hämtar den fullständiga sökvägen till filen efter arbetsbladets namn när arbetsbladet exporteras till HTML separat. Så att referenserna mellan arbetsbladen kan exporteras korrekt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Implementering av GetFullName-metoden från IFilePathProvider-gränssnittet
        public string GetFullName(string sheetName)
        {
            // För demonstration, returnera en enkel filsökväg baserad på bladnamnet
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Skapa en ny arbetsbok och lägg till lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Skapa HtmlSaveOptions och ange FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Spara arbetsboken i HTML-format
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


