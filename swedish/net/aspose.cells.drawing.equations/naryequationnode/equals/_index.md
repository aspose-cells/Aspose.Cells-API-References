---
title: "NaryEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode method. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/equals/
---
## NaryEquationNode.Equals method

Bestäm om den aktuella ekvationsnoden är lika med den angivna noden

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Den angivna noden |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hålla ekvationen
            var shape1 = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
            var equation1 = shape1.GetEquationParagraph();
            var naryNode1 = equation1.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode1 = (NaryEquationNode)naryNode1;
            naryEquationNode1.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Skapa en andra identisk form
            var shape2 = worksheet.Shapes.AddEquation(0, 100, 200, 50, 200, 50);
            var equation2 = shape2.GetEquationParagraph();
            var naryNode2 = equation2.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode2 = (NaryEquationNode)naryNode2;
            naryEquationNode2.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Skapa en tredje annan form
            var shape3 = worksheet.Shapes.AddEquation(0, 200, 200, 50, 200, 50);
            var equation3 = shape3.GetEquationParagraph();
            var naryNode3 = equation3.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode3 = (NaryEquationNode)naryNode3;
            naryEquationNode3.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            try
            {
                // Jämför identiska noder
                bool result1 = naryEquationNode1.Equals(naryEquationNode2);
                Console.WriteLine($"Comparing identical nodes: {result1}");

                // Jämför olika noder
                bool result2 = naryEquationNode1.Equals(naryEquationNode3);
                Console.WriteLine($"Comparing different nodes: {result2}");

                // Jämför med null
                bool result3 = naryEquationNode1.Equals(null);
                Console.WriteLine($"Comparing with null: {result3}");

                // Jämför med annan objekttyp
                bool result4 = naryEquationNode1.Equals("string object");
                Console.WriteLine($"Comparing with different type: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("NaryEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


