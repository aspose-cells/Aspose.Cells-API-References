---
title: "AccentEquationNode.AccentCharacterType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AccentEquationNode 属性。按类型值指定组合字符"
type: docs
url: /zh/net/aspose.cells.drawing.equations/accentequationnode/accentcharactertype/
---
## AccentEquationNode.AccentCharacterType property

通过类型值指定组合字符。

```csharp
public EquationCombiningCharacterType AccentCharacterType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class AccentEquationNodePropertyAccentCharacterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //测试获取 mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            AccentEquationNode node = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            node.AccentCharacter = "\u0302";
            node.AccentCharacterType = EquationCombiningCharacterType.GraveAccent;

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode TR = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            TR.Text = "x";
            Console.WriteLine(node.AccentCharacterType == EquationCombiningCharacterType.GraveAccent);

            workbook.Save("AccentEquationNodePropertyAccentCharacterType.xlsx");
            
        }
    }
}
```

### 另请参见

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


