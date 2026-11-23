---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "NaryEquationNode 属性。一个 nary 操作符。例如"
type: docs
url: /zh/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

an n-ary operator.e.g "∑"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
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

            // 强制转换为 NaryEquationNode 以访问 NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // 显示当前 NaryOperatorType（默认值）
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // 设置为求和操作符（∑）
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // 添加基底（操作数）和上下限以演示该操作符
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // 设置操作符随内容增长
            naryEquationNode.NaryGrow = true;

            // 更改为乘积操作符（∏）并展示差异
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // 保存工作簿
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


