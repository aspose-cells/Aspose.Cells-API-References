---
title: "NaryEquationNode.NaryGrow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode egenskap. Detta attribut specificerar tillväxt‑egenskapen för nary‑operatorer på dokumentnivå. När den är avstängd växer nary‑operatorer såsom integraler och summor inte för att matcha operandens höjd. När den är påslagen växer nary‑operatorn vertikalt för att matcha operandens höjd"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Detta attribut anger tillväxtegenskapen för n-ära operatorer på dokumentnivå. När den är av, växer n-ära operatorer såsom integraler och summor inte för att matcha operandens höjd. När den är på, växer den n-ära operatorn vertikalt för att matcha operandens höjd.

```csharp
public bool NaryGrow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ekvationsform
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Hämta ekvationsnoden
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Skapa en nary‑operatornod med NaryGrow‑egenskapen satt till true
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Lägg till nedsänkt (valfritt)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Lägg till upphöjd (valfritt)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Lägg till bas (obligatoriskt)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Spara arbetsboken
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### Se även

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


