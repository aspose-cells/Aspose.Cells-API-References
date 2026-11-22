---
title: "LowCodeSaveOptions.OutputFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptions. تحصل وتعيّن الملف مع المسار إذا لزم الأمر لحفظ البيانات المولدة. عند تعيين هذه الخاصية بقيمة غير فارغة أو غير null، سيتم تجاهل OutputStream"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

تحصل وتعيّن الملف (مع المسار إذا لزم الأمر) لحفظ البيانات المولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [`OutputStream`](../outputstream/).

```csharp
public string OutputFile { get; set; }
```

### أمثلة

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
            // إنشاء مصنف بسيط يحتوي على ورقة عمل واحدة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // حفظ بصيغ مختلفة باستخدام خاصية OutputFile
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // حفظ كملف PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // حفظ كملف JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // حفظ كـ HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // حفظ كملف CSV
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

### انظر أيضًا

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


