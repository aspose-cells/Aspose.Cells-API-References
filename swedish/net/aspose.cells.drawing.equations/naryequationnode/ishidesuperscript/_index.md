---
title: "NaryEquationNode.IsHideSuperscript"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode egenskap. Om den övre gränsen ska visas"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/
---
## NaryEquationNode.IsHideSuperscript property

Om den övre gränsen ska visas

```csharp
public bool IsHideSuperscript { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSuperscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Skapa en n-är ekvationsnod med dold upphöjd
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSuperscript = true; // Demonstrating the IsHideSuperscript property
            
            // Lägg till baskomponent
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";
            
            // Lägg till upphöjd (kommer att döljas på grund av IsHideSuperscript = true)
            EquationNode supNode = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            supText.Text = "2";

            // Spara och läs in igen för att verifiera att upphöjden är dold
            workbook.Save("NaryEquationDemo.xlsx");
            workbook = new Workbook("NaryEquationDemo.xlsx");
            
            // Verifiera den sparade ekvationen
            TextBox savedTextBox = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode savedMathNode = savedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode savedNode = (NaryEquationNode)savedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + savedNode.NaryOperator);
            Console.WriteLine("IsHideSuperscript: " + savedNode.IsHideSuperscript);
            Console.WriteLine("Superscript exists: " + (savedNode.GetChild(1).GetChild(0) != null));
        }
    }
}
```

### Se även

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


