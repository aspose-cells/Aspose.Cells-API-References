---
title: "EquationComponentNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EquationComponentNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/equationcomponentnode/equals/
---
## EquationComponentNode.Equals method

确定当前方程节点是否等于指定节点

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 指定的节点 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationComponentNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //测试获取 mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            //测试插入 Fraction
            FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            node.FractionType = EquationFractionType.Skewed;

            string str1 = "A";
            EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
            TR.Text = str1;

            string str2 = "B";
            EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
            TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
            TR.Text = str2;

            // 使用 Equals 方法比较节点
            bool areEqual = numerator?.Equals((object)denominator) ?? false;

            // 显示比较结果
            Console.WriteLine($"Nodes are equal: {areEqual}");
            workbook.Save("EquationComponentNodeMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [EquationComponentNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


