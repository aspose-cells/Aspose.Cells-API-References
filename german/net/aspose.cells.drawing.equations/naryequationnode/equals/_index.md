---
title: "NaryEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode-Methode. Bestimmt, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/equals/
---
## NaryEquationNode.Equals method

Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Der angegebene Knoten |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um die Gleichung zu enthalten
            var shape1 = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
            var equation1 = shape1.GetEquationParagraph();
            var naryNode1 = equation1.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode1 = (NaryEquationNode)naryNode1;
            naryEquationNode1.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Erstelle eine zweite identische Form
            var shape2 = worksheet.Shapes.AddEquation(0, 100, 200, 50, 200, 50);
            var equation2 = shape2.GetEquationParagraph();
            var naryNode2 = equation2.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode2 = (NaryEquationNode)naryNode2;
            naryEquationNode2.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Erstelle eine dritte unterschiedliche Form
            var shape3 = worksheet.Shapes.AddEquation(0, 200, 200, 50, 200, 50);
            var equation3 = shape3.GetEquationParagraph();
            var naryNode3 = equation3.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode3 = (NaryEquationNode)naryNode3;
            naryEquationNode3.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            try
            {
                // Identische Knoten vergleichen
                bool result1 = naryEquationNode1.Equals(naryEquationNode2);
                Console.WriteLine($"Comparing identical nodes: {result1}");

                // Unterschiedliche Knoten vergleichen
                bool result2 = naryEquationNode1.Equals(naryEquationNode3);
                Console.WriteLine($"Comparing different nodes: {result2}");

                // Vergleiche mit null
                bool result3 = naryEquationNode1.Equals(null);
                Console.WriteLine($"Comparing with null: {result3}");

                // Vergleichen mit einem anderen Objekttyp
                bool result4 = naryEquationNode1.Equals("string object");
                Console.WriteLine($"Comparing with different type: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("NaryEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


