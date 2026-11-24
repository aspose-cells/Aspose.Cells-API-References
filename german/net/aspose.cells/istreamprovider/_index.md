---
title: "Schnittstelle IStreamProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IStreamProvider Schnittstelle. Stellt den exportierten Stream‑Provider dar"
type: docs
url: /de/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Stellt den Anbieter für den exportierten Stream dar.

```csharp
public interface IStreamProvider
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Schließt den Stream. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Liest den Stream. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // Implementierung der InitStream‑Methode
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // Implementierung der CloseStream‑Methode
        public void CloseStream(StreamProviderOptions options)
        {
            // Schließe den Stream, wenn er nicht null ist
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze einige Daten im Arbeitsblatt
            worksheet.Cells["A1"].PutValue("Hello World");

            // Erstelle HtmlSaveOptions und setze den StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Lade das Arbeitsbuch aus dem HTML‑Format
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Zeige die geladenen Daten an
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


