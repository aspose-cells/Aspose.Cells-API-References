---
title: "TwoColorGradient.Variant"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TwoColorGradient 属性。获取和设置渐变变体"
type: docs
url: /zh/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

获取和设置渐变变体。

```csharp
public int Variant { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建具有初始变体的双颜色渐变
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // 创建并将样式应用于单元格 A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // 显示当前变体值
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // 修改变体值
            gradient.Variant = 2;

            // 创建并将修改后的样式应用于单元格 B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // 增大单元格高度以可视化渐变
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


