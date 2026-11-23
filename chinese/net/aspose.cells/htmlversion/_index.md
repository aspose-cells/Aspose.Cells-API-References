---
title: "枚举 HtmlVersion"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.HtmlVersion 枚举。指示在保存为 Html 格式时使用的 HTML 版本"
type: docs
url: /zh/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

指示在保存为 Html 格式时使用的 HTML 版本。

```csharp
public enum HtmlVersion
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Default | `0` | 将文档保存为符合 MS Excel 导出 HTML 的标准。 |
| XHtml | `1` | 将文档保存为符合 XHTML 1.0 Transitional 标准。 |
| Html5 | `2` | 将文档保存为符合 HTML 5 标准。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // 创建 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // 将 HTML 版本设置为 HTML5
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // 使用 HTML5 版本保存工作簿
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // 将 HTML 版本更改为 XHTML
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // 使用 XHTML 版本保存工作簿
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // 将 HTML 版本设置为默认（兼容 MS Excel）
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // 使用默认版本保存工作簿
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


