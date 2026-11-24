---
title: "NaryEquationNode.NaryGrow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode‑Eigenschaft. Dieses Attribut gibt die Wachstums‑Eigenschaft von n‑ären Operatoren auf Dokumentebene an. Wenn deaktiviert, wachsen n‑äre Operatoren wie Integrale und Summen nicht, um die Höhe ihres Operanden anzupassen. Wenn aktiviert, wächst der n‑äre Operator vertikal, um die Höhe seines Operanden zu erreichen."
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Dieses Attribut legt die Wachstums­eigenschaft von n-ären Operatoren auf Dokumentebene fest. Wenn deaktiviert, wachsen n-äre Operatoren wie Integrale und Summen nicht, um die Höhe ihrer Operanden anzupassen. Wenn aktiviert, wächst der n-äre Operator vertikal, um die Höhe seiner Operanden zu entsprechen.

```csharp
public bool NaryGrow { get; set; }
```

### Beispiele

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
            
            // Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Den Gleichungsknoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Erstelle einen nary‑Operator‑Knoten mit der NaryGrow‑Eigenschaft auf true gesetzt
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Unterindex hinzufügen (optional)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Hochstellung hinzufügen (optional)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Basis hinzufügen (erforderlich)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Speichere die Arbeitsmappe
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### Siehe auch

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


