---
title: "TwoColorGradient.Color1"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TwoColorGradient 属性。获取和设置第一个渐变颜色"
type: docs
url: /zh/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

获取和设置第一种渐变颜色。

```csharp
public Color Color1 { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // 创建带渐变填充的样式
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // 初始化双颜色渐变
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // 将渐变应用于单元格样式
            cell.SetStyle(style);
            
            // 读取初始颜色
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // 修改渐变颜色并重新应用
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // 验证更新
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // 在输出文件中进行可视化演示
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### 另请参见

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


