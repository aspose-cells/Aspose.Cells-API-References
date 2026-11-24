---
title: "HtmlSaveOptions.StreamProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Ruft den IStreamProvider zum Exportieren von Objekten ab oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Liest oder setzt den IStreamProvider für den Export von Objekten.

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
    public class HtmlSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Ein temporäres Verzeichnis für die Ausgabe erstellen
            string outputDir = Path.Combine(Path.GetTempPath(), "AsposeStreamProviderDemo");
            Directory.CreateDirectory(outputDir);

            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("StreamProvider Demo");

            // HTML-Speicheroptionen mit benutzerdefiniertem StreamProvider konfigurieren
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.StreamProvider = new ExportStreamProvider(outputDir);

            // Speichere die Arbeitsmappe als HTML
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
            // Initialisierung falls erforderlich
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            string filePath = Path.Combine(_outputDirectory, options.CustomPath);
            return new FileStream(filePath, FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implementierung wie von der Schnittstelle gefordert
        }
    }
}
```

### Siehe auch

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


