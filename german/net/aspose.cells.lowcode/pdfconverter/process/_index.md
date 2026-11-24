---
title: "PdfConverter.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfConverter-Methode. Konvertiert die angegebene Vorlagendatei in PDF"
type: docs
url: /de/net/aspose.cells.lowcode/pdfconverter/process/
---
## Process(string, string) {#process_1}

Konvertiert die angegebene Vorlagendatei in PDF.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | String | Die zu konvertierende Vorlagendatei |
| resultFile | String | Die resultierende Datei muss eine PDF-Datei sein. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class PdfConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Beispielvorlagendatei
            CreateSampleTemplate("template.xlsx");

            try
            {
                // Rufen Sie die Process-Methode mit (String, String)-Parametern direkt auf dem Typ auf
                PdfConverter.Process("template.xlsx", "output.pdf");
                
                Console.WriteLine("Successfully converted template.xlsx to output.pdf");
                Console.WriteLine($"PDF created at: {Path.GetFullPath("output.pdf")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateSampleTemplate(string fileName)
        {
            using (Workbook workbook = new Workbook())
            {
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("PDF Conversion Test");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
                workbook.Save(fileName);
            }
        }
    }
}
```

### Siehe auch

* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konvertiert Vorlagendateien in PDF

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class PdfConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Erstellen Sie einen Beispiel-Eingabestream (Excel-Datei im Speicher)
            var workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Content");
            MemoryStream template = new MemoryStream();
            workbook.Save(template, SaveFormat.Xlsx);
            template.Position = 0;

            // Ausgabeverzeichnis
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Beispiel 1: In PDF konvertieren
            Aspose.Cells.LowCode.PdfConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodePdfSaveOptions() 
                { 
                    OutputFile = outputDir + "output.pdf",
                    PdfOptions = new PdfSaveOptions()
                });

            // Beispiel 2: In HTML konvertieren
            Aspose.Cells.LowCode.HtmlConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodeSaveOptions() 
                { 
                    OutputFile = outputDir + "output.html" 
                });

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


