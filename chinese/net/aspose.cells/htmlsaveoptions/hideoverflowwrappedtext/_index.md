---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示当单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

指示当单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在单元格 A1 中设置示例文本
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // 创建并应用带有文本换行的样式
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // 获取单元格集合并应用样式
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // 设置列宽以实现文本换行
            cells.SetColumnWidth(0, 10);
            
            // 创建 HTML 保存选项并设置 HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // 使用 HTML 选项保存工作簿
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


