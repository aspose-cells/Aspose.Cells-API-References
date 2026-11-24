---
title: "StreamProviderOptions.CustomPath"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StreamProviderOptions property. Der benutzerdefinierte PfadURL, der in der erzeugten HTML-Datei für die referenzierte Quelle gespeichert wird. Wenn der Benutzer ihn nicht definiert, wird DefaultPath verwendet. Zum Beispiel werden die Tabellendaten vom Benutzer nach d/sheet001.htm gespeichert; die im Haupt‑HTML‑File verwendete URL sollte d/sheet001.htm oder ein anderer gültiger relativer Pfad sein, der vom Haupt‑HTML‑File aus zugänglich ist."
type: docs
url: /de/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

Der vom Benutzer benutzerdefinierte Pfad (URL), der in der erzeugten html-Datei für die referenzierte Quelle gespeichert wird. Wenn er nicht vom Benutzer definiert wird, wird DefaultPath verwendet. Zum Beispiel wird das Blattdaten vom Benutzer nach d:/sheet001.htm gespeichert, die in der Haupt‑html‑Datei verwendete URL sollte \"d:/sheet001.htm\" oder ein anderer gültiger relativer Pfad sein, der von der Haupt‑html‑Datei aus zugänglich ist.

```csharp
public string CustomPath { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Richten Sie HTML-Speicheroptionen mit benutzerdefiniertem Stream‑Provider ein
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // Erstellen Sie einen benutzerdefinierten Stream‑Provider mit CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Speichere die Arbeitsmappe
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Überprüfen Sie, ob der benutzerdefinierte Pfad verwendet wurde
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Vereinfachte Implementierung des benutzerdefinierten Stream‑Providers
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
            // Die Implementierung würde hier erfolgen
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Die Implementierung würde hier erfolgen
        }
    }
}
```

### Siehe auch

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


