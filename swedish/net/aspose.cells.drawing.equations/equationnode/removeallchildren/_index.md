---
title: "EquationNode.RemoveAllChildren"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode method. Tar bort alla barnnoder för den aktuella noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/removeallchildren/
---
## EquationNode.RemoveAllChildren method

Tar bort alla barnnoder för den aktuella noden.

```csharp
public void RemoveAllChildren()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveAllChildrenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hålla ekvationen
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Hämta ekvationsnoden
            var equationNode = ((TextBox)shape).GetEquationParagraph();

            // Lägg till några barnnoder till ekvationen
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            numerator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            denominator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML

            Console.WriteLine($"Equation before RemoveAllChildren: {equationNode.ToMathML()}");

            try
            {
                // Anropa RemoveAllChildren-metoden
                equationNode.RemoveAllChildren();

                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Equation after RemoveAllChildren: {equationNode.ToMathML()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAllChildren method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("EquationNodeMethodRemoveAllChildrenDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


