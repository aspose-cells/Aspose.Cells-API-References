---
title: "枚举 HtmlOfficeMathOutputType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.HtmlOfficeMathOutputType 枚举。表示如何将 OfficeMath 导出为 HTML"
type: docs
url: /zh/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

表示如何将 OfficeMath 导出为 HTML。

```csharp
public enum HtmlOfficeMathOutputType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Image | `0` | 将 OfficeMath 转换为 HTML，以 &lt;img&gt; 标签指定的图像形式。 |
| MathML | `1` | 使用 MathML 将 OfficeMath 转换为 HTML。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 将 OfficeMath 添加到单元格 A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // 创建 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // 将 OfficeMath 输出类型设置为 Image
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // 使用 Image 输出类型保存
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // 将输出类型更改为 MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // 使用 MathML 输出类型保存
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


