---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode Eigenschaft. ein n-ärer Operator. z.B."
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

Ein n-ärer Operator, z.B. \"∑\"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um die Gleichung zu enthalten
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Greifen Sie auf die Gleichung zu und fügen Sie einen n-ären Operatorknoten hinzu
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Wandeln Sie zu NaryEquationNode um, um auf NaryOperatorType zuzugreifen
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Aktuellen NaryOperatorType anzeigen (Standardwert)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Auf Summenoperator (∑) setzen
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Basis (Operand) und Grenzen hinzufügen, um den Operator zu demonstrieren
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Den Operator so einstellen, dass er mit seinem Inhalt wächst
            naryEquationNode.NaryGrow = true;

            // Auf Produktoperator (∏) umschalten und den Unterschied zeigen
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Speichere die Arbeitsmappe
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


