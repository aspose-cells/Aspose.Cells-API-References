---
title: "NaryEquationNode.IsHideSubscript"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "NaryEquationNode 属性。是否显示下界"
type: docs
url: /zh/net/aspose.cells.drawing.equations/naryequationnode/ishidesubscript/
---
## NaryEquationNode.IsHideSubscript property

是否显示下限

```csharp
public bool IsHideSubscript { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSubscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // 创建一个带隐藏下标的 Nary 方程节点
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSubscript = true; // Hide subscript
            node.IsHideSuperscript = false; // Show superscript

            // 添加下标（将被隐藏）
            EquationNode sub = node.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
            subText.Text = "1";

            // 添加上标（将可见）
            EquationNode sup = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
            supText.Text = "5";

            // 添加基底
            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
            baseText.Text = "C";

            // 保存并验证
            workbook.Save("NaryEquationDemo.xlsx");
            
            // 重新加载以验证属性
            Workbook loadedWorkbook = new Workbook("NaryEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode loadedNode = (NaryEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + loadedNode.NaryOperator);
            Console.WriteLine("IsHideSubscript: " + loadedNode.IsHideSubscript);
            Console.WriteLine("IsHideSuperscript: " + loadedNode.IsHideSuperscript);
        }
    }
}
```

### 另请参见

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


