---
title: "NaryEquationNode.LimitLocation"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "NaryEquationNode 属性。此属性指定 nary 运算符中极限的位置。极限可以居中显示在 nary 运算符的上下方，或仅位于运算符的右侧。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

此属性指定 n-ary 运算符中极限的位置。极限可以居中于 n-ary 运算符的上方和下方，或仅位于运算符的右侧。

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个用于容纳方程的形状
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // 访问方程并添加一个 nary 操作符节点
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // 将对象强制转换为 NaryEquationNode 以访问 LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // 显示当前 LimitLocation（默认值）
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // 将 LimitLocation 设置为 SubSup（右侧极限）
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // 改回 UndOvr（居中极限）
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // 保存工作簿
                workbook.Save("LimitLocationDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


