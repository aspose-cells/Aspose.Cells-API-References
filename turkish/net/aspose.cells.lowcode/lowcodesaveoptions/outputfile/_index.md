---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptions özelliği. Oluşturulan verileri kaydetmek için gerektiğinde dosya yolunu alır ve ayarlar. Bu özelliği null veya boş bir dize dışında bir değerle ayarladığınızda OutputStream yok sayılacaktır."
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile birlikte) alır ve ayarlar. Bu özelliği null veya boş bir dize dışında bir değerle ayarladığınızda, [`OutputStream`](../outputstream/) yok sayılacaktır.

```csharp
public string OutputFile { get; set; }
```

### Örnekler

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
            // Bir çalışma sayfasına sahip basit bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // OutputFile özelliğini kullanarak farklı formatlarda kaydedin
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // PDF olarak kaydedin
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // JSON olarak kaydedin
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // HTML olarak kaydet
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // CSV olarak kaydedin
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

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


