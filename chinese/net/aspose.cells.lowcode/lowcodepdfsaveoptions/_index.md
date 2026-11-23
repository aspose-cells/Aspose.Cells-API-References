---
title: "类 LowCodePdfSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodePdfSaveOptions 类。以低代码方式保存 pdf 的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

以低代码方式保存 PDF 的选项。

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | 获取并设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，[`OutputStream`](../lowcodesaveoptions/outputstream/) 将被忽略。（继承自 [`LowCodeSaveOptions`](../lowcodesaveoptions/)。） |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | 获取并设置用于写入生成数据的流。当将此属性设置为非 null 时，[`OutputFile`](../lowcodesaveoptions/outputfile/) 将被忽略。（继承自 [`LowCodeSaveOptions`](../lowcodesaveoptions/)。） |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | 用于保存 Pdf 文件的选项。 |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | 输出的保存格式。对于转换为 pdf，只能是 Pdf。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // 创建示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // 创建 PDF 保存选项
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // 创建低代码 PDF 保存选项
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // 使用低代码选项保存
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


