---
title: "DelimiterEquationNode.NaryGrow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DelimiterEquationNode egenskap. Anger om avgränsaren automatiskt ska expandera och kontrahera med formelns höjd"
type: docs
url: /sv/net/aspose.cells.drawing.equations/delimiterequationnode/narygrow/
---
## DelimiterEquationNode.NaryGrow property

Specificerar om avgränsaren automatiskt ska expandera och kontrahera med formelns höjd.

```csharp
public bool NaryGrow { get; set; }
```

### Anmärkningar

Denna egenskap specificerar tillväxtegenskapen för avgränsaren på dokumentnivå. När den är avstängd kommer avgränsaren inte att växa för att matcha storleken på dess komponenthöjd. När den är aktiverad växer avgränsaren vertikalt för att matcha dess komponenthöjd.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            var paragraph = textBox.GetEquationParagraph();
            var mathNode = paragraph.GetChild(0);
            
            // Skapa avgränsningsnod med NaryGrow‑egenskap
            var delimiterNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Delimiter) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            delimiterNode.DelimiterShape = Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType.Match;
            delimiterNode.NaryGrow = false; // Demonstrating NaryGrow property
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            delimiterNode.SeparatorChar = ",";

            // Lägg till baselement
            var baseNode1 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode1 = baseNode1.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode1.Text = "x";

            var baseNode2 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode2 = baseNode2.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode2.Text = "y";

            // Spara och verifiera
            string outputFile = "DelimiterEquationNode_NaryGrow_Demo.xlsx";
            workbook.Save(outputFile);

            // Verifiera den sparade filen
            Workbook verifyWorkbook = new Workbook(outputFile);
            var verifyTextBox = verifyWorkbook.Worksheets[0].Shapes[0] as Aspose.Cells.Drawing.TextBox;
            var verifyNode = verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            
            Console.WriteLine("NaryGrow value: " + verifyNode.NaryGrow); // Should output "False"
        }
    }
}
```

### Se även

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


