---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptions-egenskap. Hämtar och anger filen med sökväg om det behövs för att spara den genererade datan. När denna egenskap sätts till ett värde annat än null eller en tom sträng kommer OutputStream att ignoreras."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Hämtar och anger filen (med sökväg om det behövs) för att spara den genererade datan. När denna egenskap sätts till ett värde annat än null eller en tom sträng, kommer [`OutputStream`](../outputstream/) att ignoreras.

```csharp
public string OutputFile { get; set; }
```

### Exempel

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
            // Skapa en enkel arbetsbok med ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Spara till olika format med OutputFile-egenskapen
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Spara som PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // Spara som JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // Spara som HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // Spara som CSV
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

### Se även

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


