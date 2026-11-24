---
title: "NaryEquationNode.IsHideSubscript"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode Eigenschaft. Ob die untere Grenze angezeigt werden soll"
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/ishidesubscript/
---
## NaryEquationNode.IsHideSubscript property

Ob die untere Grenze angezeigt werden soll

```csharp
public bool IsHideSubscript { get; set; }
```

### Beispiele

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
            
            // Erstellen Sie einen Nary-Gleichungsknoten mit verstecktem Tiefstellen
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSubscript = true; // Hide subscript
            node.IsHideSuperscript = false; // Show superscript

            // Tiefstellen hinzufügen (wird versteckt)
            EquationNode sub = node.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
            subText.Text = "1";

            // Hochstellen hinzufügen (wird sichtbar)
            EquationNode sup = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
            supText.Text = "5";

            // Basis hinzufügen
            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
            baseText.Text = "C";

            // Speichern und überprüfen
            workbook.Save("NaryEquationDemo.xlsx");
            
            // Neu laden, um Eigenschaften zu überprüfen
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

### Siehe auch

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


