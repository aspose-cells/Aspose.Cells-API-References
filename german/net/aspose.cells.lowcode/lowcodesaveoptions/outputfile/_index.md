---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptions-Eigenschaft. Gibt den Dateipfad zurück und legt ihn fest, falls für das Speichern der erzeugten Daten erforderlich. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird OutputStream ignoriert."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Gibt die Datei (mit Pfad, falls erforderlich) für das Speichern der erzeugten Daten zurück und legt sie fest. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird [`OutputStream`](../outputstream/) ignoriert.

```csharp
public string OutputFile { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeSaveOptionsPropertyOutputFileDemo
    {
        public static void Run()
        {
            // Erstelle ein einfaches Workbook mit einem Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Speichere in verschiedene Formate unter Verwendung der OutputFile-Eigenschaft
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Als PDF speichern
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // Als JSON speichern
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // Als HTML speichern
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // Als CSV speichern
            SaveWithOutputFile(workbook, SaveFormat.Csv, "output.csv");
        }

        private static void SaveWithOutputFile(Workbook workbook, SaveFormat format, string fileName)
        {
            string outputPath = "Output/" + fileName;
            
            switch (format)
            {
                case SaveFormat.Pdf:
                    PdfConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodePdfSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Json:
                    JsonConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Html:
                    HtmlConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                case SaveFormat.Csv:
                    TextConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
                        new LowCodeSaveOptions { OutputFile = outputPath });
                    break;
                default:
                    throw new NotSupportedException("Format not supported: " + format);
            }

            Console.WriteLine($"File saved successfully to: {outputPath}");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


