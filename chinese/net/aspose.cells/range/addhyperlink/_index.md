---
title: "Range.AddHyperlink"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。向指定单元格或单元格范围添加超链接"
type: docs
url: /zh/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

向指定的单元格或单元格范围添加超链接。

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | String | 超链接的地址。 |
| textToDisplay | String | 指定超链接要显示的文本。 |
| screenTip | String | 指定超链接的屏幕提示文本。 |

### 返回值

[`Hyperlink`](../../hyperlink/) object.

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // 添加带有地址、显示文本和屏幕提示的超链接
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // 保存工作簿
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


