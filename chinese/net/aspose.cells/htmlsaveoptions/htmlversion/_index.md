---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指定在保存 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

指定在保存 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default。

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加一些示例数据
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // 创建 HtmlSaveOptions 实例
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // 显示当前 HtmlVersion 值
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // 将 HtmlVersion 设置为 HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // 使用 HTML5 版本保存
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // 切换为 XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // 使用 XHTML 版本保存
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // 重置为默认值
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // 使用默认版本保存
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### 另请参见

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


