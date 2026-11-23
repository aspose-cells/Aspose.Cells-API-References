---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GroupCharacterEquationNode 属性。此属性与 groupChrPr 的 pos 结合，指定 groupChr 对象的垂直布局。其中 pos 指定分组字符的位置，vertJc 指定对象相对于基线的对齐方式。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

This attribute, combined with pos of groupChrPr, specifies the vertical layout of the groupChr object. Where pos specifies the position of the grouping character, vertJc specifies the alignment of the object with respect to the baseline.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个文本框形状以容纳该公式
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // 创建一个 GroupCharacterEquationNode 实例
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // 设置公式节点的初始属性
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // 演示 VertJc 属性（读写）
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // 更改 VertJc 值
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // 保存工作簿
                workbook.Save("VertJcDemo.xlsx");
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

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


