---
title: "EquationComponentNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationComponentNode metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationcomponentnode/equals/
---
## EquationComponentNode.Equals method

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

    public class EquationComponentNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //testa hämta mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            //testa infoga Fraction
            FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            node.FractionType = EquationFractionType.Skewed;

            string str1 = "A";
            EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
            TR.Text = str1;

            string str2 = "B";
            EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
            TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
            TR.Text = str2;

            // Jämför noderna med Equals-metoden
            bool areEqual = numerator?.Equals((object)denominator) ?? false;

            // Visa jämförelsens resultat
            Console.WriteLine($"Nodes are equal: {areEqual}");
            workbook.Save("EquationComponentNodeMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationComponentNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


