---
title: "AccentEquationNode.AccentCharacterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AccentEquationNode. Укажите комбинирующие символы по значению типа"
type: docs
url: /ru/net/aspose.cells.drawing.equations/accentequationnode/accentcharactertype/
---
## AccentEquationNode.AccentCharacterType property

Укажите комбинирующие символы по значению типа.

```csharp
public EquationCombiningCharacterType AccentCharacterType { get; set; }
```

### Примеры

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

            //тест get mathnode
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

### См. также

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


