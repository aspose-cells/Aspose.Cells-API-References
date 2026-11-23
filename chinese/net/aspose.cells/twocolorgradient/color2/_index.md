---
title: "TwoColorGradient.Color2"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TwoColorGradient 属性。获取和设置第二个渐变颜色"
type: docs
url: /zh/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

获取和设置第二种渐变颜色。

```csharp
public Color Color2 { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建双颜色渐变实例
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // 创建第一个样式并使用初始渐变
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // 显示当前 Color2 值
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // 修改 Color2 属性
            gradient.Color2 = Color.Red;

            // 创建第二个样式并使用修改后的渐变
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // 调整行以便可见
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // 保存工作簿
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### 另请参见

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


