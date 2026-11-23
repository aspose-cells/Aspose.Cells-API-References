---
title: "HtmlSaveOptions.CssStyles"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置格式化程序的附加 css 样式。仅在 SaveAsSingleFile 为 True 时有效。  CssStylesbody  padding 5px"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

获取或设置格式化程序的附加 css 样式。仅在 [`SaveAsSingleFile`](../saveassinglefile/) 为 True 时有效。  CssStyles=\"body { padding: 5px }\";

```csharp
public string CssStyles { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // 创建 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // 设置自定义 CSS 样式
            saveOptions.CssStyles = @"
                body { 
                    font-family: Arial;
                    background-color: #f0f0f0;
                }
                table {
                    border-collapse: collapse;
                    width: 100%;
                }
                td {
                    border: 1px solid #ddd;
                    padding: 8px;
                }";

            // 使用自定义 CSS 样式保存工作簿
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


