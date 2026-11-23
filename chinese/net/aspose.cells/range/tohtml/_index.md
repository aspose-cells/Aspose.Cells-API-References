---
title: "Range.ToHtml"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。将范围转换为 html"
type: docs
url: /zh/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

将范围转换为 html。

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | 将范围转换为 html 的选项。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在范围 A1:J25 中填充一些数据
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // 使用完全限定类型名称创建范围
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // 创建 HTML 保存选项
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // 将范围转换为 HTML
            byte[] htmlData = range.ToHtml(options);
            
            // 将 HTML 保存到文件
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


