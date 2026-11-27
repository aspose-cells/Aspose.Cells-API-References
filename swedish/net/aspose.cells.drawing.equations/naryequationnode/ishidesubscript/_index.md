---
title: "NaryEquationNode.IsHideSubscript"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode egenskap. Om den nedre gränsen ska visas"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/ishidesubscript/
---
## NaryEquationNode.IsHideSubscript property

Om den nedre gränsen ska visas

```csharp
public bool IsHideSubscript { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSubscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Skapa en Nary-ekvationsnod med dold nedsänkt
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSubscript = true; // Hide subscript
            node.IsHideSuperscript = false; // Show superscript

            // Lägg till nedsänkt (kommer att döljas)
            EquationNode sub = node.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
            subText.Text = "1";

            // Lägg till upphöjd (kommer att vara synlig)
            EquationNode sup = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
            supText.Text = "5";

            // Lägg till bas
            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
            baseText.Text = "C";

            // Spara och verifiera
            workbook.Save("NaryEquationDemo.xlsx");
            
            // Läs om för att verifiera egenskaper
            Workbook loadedWorkbook = new Workbook("NaryEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode loadedNode = (NaryEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + loadedNode.NaryOperator);
            Console.WriteLine("IsHideSubscript: " + loadedNode.IsHideSubscript);
            Console.WriteLine("IsHideSuperscript: " + loadedNode.IsHideSuperscript);
        }
    }
}
```

### Se även

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


