---
title: "LowCodeSaveOptions.OutputFile"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptions 属性。获取和设置用于保存生成数据的文件（包括路径），如果需要。当将此属性设置为非 null 或空字符串时，OutputStream 将被忽略"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

获取和设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或空字符串时，[`OutputStream`](../outputstream/) 将被忽略。

```csharp
public string OutputFile { get; set; }
```

### 示例

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
            // 创建一个包含一个工作表的简单工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // 使用 OutputFile 属性保存为不同格式
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // 另存为 PDF
            SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");

            // 另存为 JSON
            SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");

            // 另存为 HTML
            SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");

            // 另存为 CSV
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

### 另请参见

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


