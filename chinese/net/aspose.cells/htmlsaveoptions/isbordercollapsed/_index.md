---
title: "HtmlSaveOptions.IsBorderCollapsed"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示表格边框是否已折叠。默认值为 true"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/isbordercollapsed/
---
## HtmlSaveOptions.IsBorderCollapsed property

指示表格边框是否已折叠。默认值为 true。

```csharp
public bool IsBorderCollapsed { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsBorderCollapsedDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据和边框
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("With Borders");
            worksheet.Cells["B2"].SetStyle(style);

            // 设置演示的区域设置
            var culture = new System.Globalization.CultureInfo("de-DE");
            Thread.CurrentThread.CurrentCulture = culture;
            Thread.CurrentThread.CurrentUICulture = culture;
            workbook.Settings.CultureInfo = culture;

            // 创建 HTML 保存选项并设置 IsBorderCollapsed
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;

            // 使用 HTML 选项保存工作簿
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "HtmlWithBorders.html");
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("File saved with collapsed borders: " + outputPath);
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


