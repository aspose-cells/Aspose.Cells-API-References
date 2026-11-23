---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示当单元格内容溢出列时是否显示整个格式化数据。如果为 true，则忽略列宽并导出单元格的全部数据。如果为 false，则数据的导出方式与 Excel 相同。默认值为 false"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

指示当单元格内容溢出列时是否显示整个格式化数据。如果为 true，则忽略列宽并导出单元格的全部数据。如果为 false，则数据的导出方式与 Excel 相同。默认值为 false。

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 设置示例数据和列宽
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // 创建 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // 演示 FormatDataIgnoreColumnWidth 属性
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // 使用不同设置保存以展示效果
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


