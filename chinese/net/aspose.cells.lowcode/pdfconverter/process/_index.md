---
title: "PdfConverter.Process"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PdfConverter 方法。将给定的模板文件转换为 pdf"
type: docs
url: /zh/net/aspose.cells.lowcode/pdfconverter/process/
---
## Process(string, string) {#process_1}

将给定的模板文件转换为 PDF。

```csharp
public static void Process(string templateFile, string resultFile)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | String | 待转换的模板文件 |
| resultFile | String | 生成的文件必须是 pdf 文件。 |

### 示例

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
            // 创建示例模板文件
            CreateSampleTemplate("template.xlsx");

            try
            {
                // 在类型上直接使用 (String, String) 参数调用 Process 方法
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

### 另请参见

* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

将模板文件转换为 PDF

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | 输入和加载的选项 |
| saveOptions | LowCodeSaveOptions | 输出和保存的选项 |

### 示例

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
            // 创建示例输入流（内存中的 Excel 文件）
            var workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Content");
            MemoryStream template = new MemoryStream();
            workbook.Save(template, SaveFormat.Xlsx);
            template.Position = 0;

            // 输出目录
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            // 示例 1：转换为 PDF
            Aspose.Cells.LowCode.PdfConverter.Process(
                new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
                new Aspose.Cells.LowCode.LowCodePdfSaveOptions() 
                { 
                    OutputFile = outputDir + "output.pdf",
                    PdfOptions = new PdfSaveOptions()
                });

            // 示例 2：转换为 HTML
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

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


