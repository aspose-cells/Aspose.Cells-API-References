---
title: "Style.Style"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 构造函数。初始化 Style 类的新实例"
type: docs
url: /zh/net/aspose.cells/style/style/
---
## Style constructor

初始化 [`Style`](../) 类的新实例。

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### 备注

注意：此构造函数已过时。请改用 CellsFactory.CreateStyle() 方法。此属性将在自 2016 年 10 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 使用构造函数创建样式
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // 将样式应用于单元格
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // 保存工作簿
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


