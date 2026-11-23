---
title: "AccentEquationNode.Equals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AccentEquationNode 方法。确定当前方程节点是否等于指定的节点"
type: docs
url: /zh/net/aspose.cells.drawing.equations/accentequationnode/equals/
---
## AccentEquationNode.Equals method

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

    public class AccentEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //测试获取 mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            AccentEquationNode node = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            node.AccentCharacter = "\u0302";

            AccentEquationNode node2 = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            node2.AccentCharacter = "\u0302";

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            TR.Text = "x";

            EquationNode subBase2 = node2.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR2 = (TextRunEquationNode)(subBase2.AddChild(EquationNodeType.Text));
            TR2.Text = "y";
            Console.WriteLine("AccentEquationNode.Equals(Object) method is called: " + node.Equals(node2));

            workbook.Save("AccentEquationNodeMethodEquals.xlsx");
           
        }
    }
}
```

### 另请参见

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


