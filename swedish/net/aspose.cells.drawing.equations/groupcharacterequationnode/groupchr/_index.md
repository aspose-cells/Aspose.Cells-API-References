---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupCharacterEquationNode egenskap. Anger ett symbolstandard U23DF. Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd den här egenskapsinställningen om du inte kan hitta tecknet du behöver i en känd typ"
type: docs
url: /sv/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Anger en symbol (standard U+23DF). Det rekommenderas starkt att använda attributet ChrType för att ange accenttecken. Använd denna egenskapsinställning om du inte kan hitta tecknet du behöver i en känd typ.

```csharp
public string GroupChr { get; set; }
```

### Anmärkningar

Det bör noteras att denna egenskap endast accepterar ett tecken, och om flera tecken skickas in, accepteras endast det första tecknet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvation i det första kalkylbladet
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Hämta ekvationens rotnod
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Skapa en gruppteckennod med dubbelpil åt höger
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Lägg till grundtext till grupptecknet
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // Demonstrera användning av GroupChr egenskap
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Spara arbetsboken
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


