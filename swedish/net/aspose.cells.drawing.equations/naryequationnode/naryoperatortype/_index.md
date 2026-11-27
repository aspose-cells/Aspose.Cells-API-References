---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode egenskap. en n-är operator.t.ex"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

en n-är operator.t.ex \"∑\"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hålla ekvationen
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Få åtkomst till ekvationen och lägg till en n-är operatornod
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Kasta till NaryEquationNode för att komma åt NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Visa aktuell NaryOperatorType (standardvärde)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Ställ in till summationsoperator (∑)
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Lägg till bas (operand) och gränser för att demonstrera operatorn
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Ställ in operatorn att växa med sitt innehåll
            naryEquationNode.NaryGrow = true;

            // Byt till produktoperator (∏) och visa skillnaden
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Spara arbetsboken
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


