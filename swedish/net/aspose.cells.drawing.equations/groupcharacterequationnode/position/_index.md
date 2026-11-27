---
title: "GroupCharacterEquationNode.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupCharacterEquationNode property. Detta attribut specificerar tecknets position i objektet"
type: docs
url: /sv/net/aspose.cells.drawing.equations/groupcharacterequationnode/position/
---
## GroupCharacterEquationNode.Position property

Detta attribut anger tecknets position i objektet

```csharp
public EquationCharacterPositionType Position { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvationsform till det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationsstycket och lägg till en gruppteckensnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Ställ in positionsegenskapen (grundläggande demonstration)
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Lägg till bastext
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";

            // Spara arbetsboken
            string outputPath = "GroupCharacterEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Equation with group character position set to Top has been created successfully.");
        }
    }
}
```

### Se även

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


