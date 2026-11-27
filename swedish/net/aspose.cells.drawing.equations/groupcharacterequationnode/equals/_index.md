---
title: "GroupCharacterEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupCharacterEquationNode metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/groupcharacterequationnode/equals/
---
## GroupCharacterEquationNode.Equals method

Bestäm om den aktuella ekvationsnoden är lika med den angivna noden

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Den angivna noden |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två GroupCharacterEquationNode-instanser för jämförelse
            // Eftersom GroupCharacterEquationNode inte har en parameterlös konstruktor,
            // måste vi skapa dem via kalkylbladets ShapeCollection
            var shape1 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node1 = (GroupCharacterEquationNode)shape1.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node1.GroupChr = "⏟";
            node1.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node1.Position = EquationCharacterPositionType.Bottom;
            node1.VertJc = EquationCharacterPositionType.Bottom;

            var shape2 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node2 = (GroupCharacterEquationNode)shape2.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node2.GroupChr = "⏟";
            node2.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node2.Position = EquationCharacterPositionType.Bottom;
            node2.VertJc = EquationCharacterPositionType.Bottom;

            try
            {
                // Anropa Equals-metoden med Object-parameter
                bool areEqual = node1.Equals((Object)node2);

                // Visa jämförelsens resultat
                Console.WriteLine($"The two GroupCharacterEquationNode instances are equal: {areEqual}");

                // Lägg till resultatet i kalkylbladet
                worksheet.Cells["A1"].PutValue("GroupCharacterEquationNode Equals Comparison Result:");
                worksheet.Cells["A2"].PutValue(areEqual);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("GroupCharacterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


