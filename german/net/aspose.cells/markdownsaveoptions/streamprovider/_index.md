---
title: "MarkdownSaveOptions.StreamProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Gibt den IStreamProvider für den Export von Objekten zurück oder legt ihn fest. Wenn null, werden die exportierten Objekte im selben Verzeichnis wie die Ausgabedatei gespeichert."
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/streamprovider/
---
## MarkdownSaveOptions.StreamProvider property

Liest oder setzt den IStreamProvider zum Exportieren von Objekten. Wenn `null`, werden die exportierten Objekte im selben Verzeichnis wie die Ausgabedatei gespeichert.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Hello";
            worksheet.Cells["B1"].Value = "World";

            try
            {
                // Erstelle eine MarkdownSaveOptions-Instanz.
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Zeige den aktuellen StreamProvider-Wert an (standardmäßig null).
                Console.WriteLine("Current StreamProvider: " + (saveOptions.StreamProvider == null ? "null" : "set"));

                // Erstelle eine benutzerdefinierte StreamProvider-Implementierung.
                CustomStreamProvider streamProvider = new CustomStreamProvider();
                saveOptions.StreamProvider = streamProvider;

                // Den aktualisierten StreamProvider-Wert anzeigen
                Console.WriteLine("Updated StreamProvider: " + (saveOptions.StreamProvider != null ? "set" : "null"));

                // Speichere die Arbeitsmappe mit dem benutzerdefinierten StreamProvider
                workbook.Save("StreamProviderDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved with custom StreamProvider.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    // Benutzerdefinierte Implementierung von IStreamProvider
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

### Siehe auch

* interface [IStreamProvider](../../istreamprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


