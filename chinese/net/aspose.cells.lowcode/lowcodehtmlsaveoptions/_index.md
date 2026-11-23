---
title: "类 LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.LowCodeHtmlSaveOptions 类。以低代码方式保存 HTML 的选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

以低代码方式保存 HTML 的选项。

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | 保存 HTML 的通用选项。 |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | 获取并设置用于保存生成数据的文件（如有需要包括路径）。当将此属性设置为非 null 或非空字符串时，[`OutputStream`](../lowcodesaveoptions/outputstream/) 将被忽略。（继承自 [`LowCodeSaveOptions`](../lowcodesaveoptions/)。） |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | 获取并设置用于写入生成数据的流。当将此属性设置为非 null 时，[`OutputFile`](../lowcodesaveoptions/outputfile/) 将被忽略。（继承自 [`LowCodeSaveOptions`](../lowcodesaveoptions/)。） |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | 获取和设置电子表格的格式。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // 创建并配置 LowCodeHtmlSaveOptions
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // 使用保存选项参数，利用已配置的 HTML 选项保存工作簿
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


