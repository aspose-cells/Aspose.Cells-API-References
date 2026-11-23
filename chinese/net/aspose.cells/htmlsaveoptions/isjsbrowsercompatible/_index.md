---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // 将 IsJsBrowserCompatible 设置为 true，以配置 HTML 保存选项。
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // 以 JavaScript 兼容性保存工作簿。
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


