---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。指示 OfficeMath 对象如何导出为 Markdown。默认值为 Image"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

指示 OfficeMath 对象如何导出为 Markdown，默认值为 Image。

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加包含可能含有 OfficeMath 的公式的示例数据
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // 创建 Markdown 保存选项
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // 显示 OfficeMathOutputType 的当前值
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // 将 OfficeMathOutputType 设置为 MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // 以 MathML 输出类型保存工作簿
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // 更改为 Image 输出类型
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // 以 Image 输出类型保存工作簿
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


