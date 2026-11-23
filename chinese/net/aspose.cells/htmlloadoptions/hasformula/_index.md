---
title: "HtmlLoadOptions.HasFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlLoadOptions 属性。指示如果文本以...开头则是否为公式"
type: docs
url: /zh/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

指示文本是否为公式（如果以 "=" 开头）。

```csharp
public bool HasFormula { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // 将 HasFormula 设置为 false，以将公式字符串视为纯文本
            loadOptions.HasFormula = false;
            
            // 使用 HTML 文件和加载选项创建工作簿
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // 显示一些单元格值以演示 HTML 导入
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // 另存为 XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


