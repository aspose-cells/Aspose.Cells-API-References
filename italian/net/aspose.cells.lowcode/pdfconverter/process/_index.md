---
title: "PdfConverter.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PdfConverter. Converte il file modello fornito in pdf"
type: docs
url: /it/net/aspose.cells.lowcode/pdfconverter/process/
---
## Process(string, string) {#process_1}

Converte il file modello fornito in PDF.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da convertire |
| resultFile | String | Il file risultante, deve essere un file pdf. |

### Esempi

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
            // Crea un file modello di esempio
            CreateSampleTemplate("template.xlsx");

            try
            {
                // Chiama il metodo Process con parametri (String, String) direttamente sul tipo
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

### Vedi anche

* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converte il file modello in PDF

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |

### Esempi

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
            // Crea un stream di input di esempio (file Excel in memoria)
            var workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Content");
            MemoryStream template = new MemoryStream();
            workbook.Save(template, SaveFormat.Xlsx);
            template.Position = 0;

            // Directory di destinazione
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Esempio 1: Converti in PDF
            Aspose.Cells.LowCode.PdfConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodePdfSaveOptions() 
                { 
                    OutputFile = outputDir + "output.pdf",
                    PdfOptions = new PdfSaveOptions()
                });

            // Esempio 2: Converti in HTML
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

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


