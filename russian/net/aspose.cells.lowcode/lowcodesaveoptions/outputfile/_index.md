---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptions. Получает и задает filewith путь, если необходимо, для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, свойство OutputStream будет игнорироваться"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Получает и задает файл (с путем, если необходимо) для сохранения сгенерированных данных. При установке этого свойства значением, отличным от null или пустой строки, [`OutputStream`](../outputstream/) будет игнорироваться.

```csharp
public string OutputFile { get; set; }
```

### Примеры

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
            // Создать простую книгу с одним листом
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Сохранить в разных форматах, используя свойство OutputFile
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // Сохранить как PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // Сохранить как JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // Сохранить как HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // Сохранить как CSV
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

### См. также

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


