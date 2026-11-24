---
title: "NaryEquationNode.IsHideSuperscript"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode Eigenschaft. Ob die obere Grenze angezeigt werden soll"
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/
---
## NaryEquationNode.IsHideSuperscript property

Ob die obere Grenze angezeigt werden soll

```csharp
public bool IsHideSuperscript { get; set; }
```

### Beispiele

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
            
            // Erstellen Sie einen n-ären Gleichungsknoten mit versteckter Hochstellung
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSuperscript = true; // Demonstrating the IsHideSuperscript property
            
            // Basiskomponente hinzufügen
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";
            
            // Hochstellen hinzufügen (wird versteckt, weil IsHideSuperscript = true)
            EquationNode supNode = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            supText.Text = "2";

            // Speichern und neu laden, um zu überprüfen, dass die Hochstellung versteckt ist
            workbook.Save("NaryEquationDemo.xlsx");
            workbook = new Workbook("NaryEquationDemo.xlsx");
            
            // Gespeicherte Gleichung überprüfen
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

### Siehe auch

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


