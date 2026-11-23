---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GroupCharacterEquationNode 属性。指定符号默认值 U23DF。强烈建议使用属性 ChrType 来设置重音字符。如果在已知类型中找不到所需字符，请使用此属性设置。"
type: docs
url: /zh/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Specifies a symbol(default U+23DF). It is strongly recommended to use attribute ChrType to set accent character. Use this property setting if you cannot find the character you need in a known type.

```csharp
public string GroupChr { get; set; }
```

### 备注

需要注意的是，此属性仅接受一个字符，如果传入多个字符，只会接受第一个字符。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 在第一个工作表中添加公式
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // 获取公式的根节点
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // 创建一个带有向右双箭头的组字符节点
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // 向组字符添加基础文本
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // 演示 GroupChr 属性的用法
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // 保存工作簿
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


