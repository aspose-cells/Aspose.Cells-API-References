---
title: "NaryEquationNode.NaryOperator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode-Eigenschaft. ein närer Operator, z.B. . Es wird dringend empfohlen, das Attribut NaryOperatorType zu verwenden, um den nären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können."
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

Ein n-ärer Operator, z.B. \"∑\". Es wird dringend empfohlen, das Attribut NaryOperatorType zu verwenden, um den n-ären Operator festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

```csharp
public string NaryOperator { get; set; }
```

### Hinweise

Es sollte beachtet werden, dass diese Eigenschaft nur ein Zeichen akzeptiert und bei mehreren übergebenen Zeichen nur das erste Zeichen verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Den Gleichungsknoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Erstelle einen nären Operator-Knoten
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Setze nary operator-Eigenschaften
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Unterindex hinzufügen (optional)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Hochstellung hinzufügen (optional)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Basisausdruck hinzufügen
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Speichere die Arbeitsmappe
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### Siehe auch

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


