---
title: "Style.ToJson"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 方法。将 Style 转换为 JSON 结构数据"
type: docs
url: /zh/net/aspose.cells/style/tojson/
---
## Style.ToJson method

将 [`Style`](../) 转换为 JSON 结构数据。

```csharp
public string ToJson()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 创建并将样式应用于单元格 B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // 将样式转换为 JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // 在单元格 B6 中设置公式
            cells["B6"].Formula = "=A1";

            // 将单元格转换为 JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


