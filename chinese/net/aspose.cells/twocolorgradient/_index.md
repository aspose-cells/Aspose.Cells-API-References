---
title: "类 TwoColorGradient"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.TwoColorGradient 类。表示双颜色渐变"
type: docs
url: /zh/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

表示双颜色渐变。

```csharp
public class TwoColorGradient
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | 获取和设置第一种渐变颜色。 |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | 获取和设置第二种渐变颜色。 |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | 获取和设置渐变阴影样式。 |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | 获取和设置渐变变体。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 使用构造函数参数初始化 TwoColorGradient
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // 在初始化后修改渐变属性
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // 创建单元格样式并应用渐变
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // 将样式应用于单元格并添加内容
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // 调整单元格尺寸以便可见
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // 保存带有渐变格式的结果
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


