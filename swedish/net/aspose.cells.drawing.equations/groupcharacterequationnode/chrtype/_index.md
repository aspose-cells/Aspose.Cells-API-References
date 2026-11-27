---
title: "GroupCharacterEquationNode.ChrType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupCharacterEquationNode property. Specificera kombinationstecken efter typvärde"
type: docs
url: /sv/net/aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/
---
## GroupCharacterEquationNode.ChrType property

Specificera kombinerande tecken med typvärde.

```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyChrTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvation i det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta ekvationens rotnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Lägg till en gruppteckensnod
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Ställ in gruppteckenegenskaper
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Lägg till bastext
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "test";

            // Spara arbetsboken
            workbook.Save("GroupCharacterEquationDemo.xlsx");

            // Verifiera den sparade filen
            Workbook verifyWorkbook = new Workbook("GroupCharacterEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            GroupCharacterEquationNode verifyNode = (GroupCharacterEquationNode)verifyTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);

            Console.WriteLine("Group Character Type: " + verifyNode.ChrType);
            Console.WriteLine("Group Character: " + verifyNode.GroupChr);
            Console.WriteLine("Base Text: " + ((TextRunEquationNode)verifyNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Se även

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


