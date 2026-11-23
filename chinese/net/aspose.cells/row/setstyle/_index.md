---
title: "Row.SetStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Row 方法。设置此行的样式"
type: docs
url: /zh/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

设置此行的样式。

```csharp
public void SetStyle(Style style)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 样式 | 样式 | 此行中单元格使用的默认样式。 |

### 备注

此方法仅将给定的样式设置为此行的默认样式，而不更改此行中已有单元格的样式设置。若要同时将已有单元格的样式设置更新为指定样式，请使用 [`ApplyStyle`](../applystyle/)

### 示例

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建并配置样式
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // 获取第一行并应用样式
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // 保存工作簿
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


