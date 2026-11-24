---
title: "HtmlLoadOptions.StreamProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt den StreamProviderImportHtmlFile zum Importieren von Objekten zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Liest oder setzt den StreamProviderImportHtmlFile zum Importieren von Objekten.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Beispiele

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
            // Initialisieren Sie den Stream bei Bedarf.
        }

        public Stream ProvideStream(StreamProviderOptions options)
        {
            // Geben Sie einen Stream zum Lesen/Schreiben zurück.
            return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Schließen Sie den Stream.
            options.Stream.Close();
        }

        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");

            // Speichern mit benutzerdefiniertem StreamProvider.
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            workbook.Save("output.html", saveOptions);

            // Laden mit benutzerdefiniertem StreamProvider.
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("output.html", loadOptions);

            // Geladene Daten überprüfen.
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Siehe auch

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


