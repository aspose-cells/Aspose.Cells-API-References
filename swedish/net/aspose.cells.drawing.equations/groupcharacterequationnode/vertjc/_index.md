---
title: "GroupCharacterEquationNode.VertJc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupCharacterEquationNode egenskap. Detta attribut kombinerat med pos för groupChrPr specificerar den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet specificerar vertJc justeringen av objektet i förhållande till baslinjen"
type: docs
url: /sv/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

Detta attribut, kombinerat med pos för groupChrPr, anger den vertikala layouten för groupChr-objektet. Där pos anger positionen för grupperingstecknet, anger vertJc justeringen av objektet i förhållande till baslinjen.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en textrutaform för att innehålla ekvationen
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // Skapa en GroupCharacterEquationNode-instans
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // Ställ in initiala egenskaper för ekvationsnoden
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // Demonstrera VertJc egenskap (läsa och skriva)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // Ändra VertJc-värdet
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // Spara arbetsboken
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

### Se även

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


