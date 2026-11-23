---
title: "LoadOptions.StandardFontSize"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LoadOptions 属性。设置默认的标准字体大小"
type: docs
url: /zh/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

设置默认的标准字体大小。

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### 备注

注意：此成员现已过时。请改用 DefaultStyleSettings。此属性将在自 2022 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项并设置 StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // 使用这些选项加载工作簿
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // 访问第一个工作表和单元格
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // 设置一些示例文本并验证字体属性
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


