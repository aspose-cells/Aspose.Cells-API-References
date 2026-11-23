---
title: "类 PdfConverter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.PdfConverter 类。用于将模板文件转换为 PDF 的转换器"
type: docs
url: /zh/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

用于将模板文件转换为 PDF 的转换器。

```csharp
public class PdfConverter
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | 将模板文件转换为 PDF |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | 将给定的模板文件转换为 PDF。 |

### 示例

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // 使用模板路径和输出路径初始化 PdfConverter
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


