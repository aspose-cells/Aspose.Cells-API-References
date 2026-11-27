---
title: "EquationNode.ToMathML"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode-metod. Konvertera denna ekvation till ett MathML-uttryck"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/tomathml/
---
## EquationNode.ToMathML method

Konvertera denna ekvation till MathML-uttryck.

```csharp
public string ToMathML()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToMathMLDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en ekvationsform – lade till breddparameter (300) och höjdparameter (100)
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // Bygg en enkel ekvation: (a+b)^2 = a^2 + 2ab + b^2
            var equationNode = equation.AddChild(EquationNodeType.Text);
            var textNode = equationNode as TextRunEquationNode;
            textNode.Text = "(";

            var variableA = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableA.Text = "a";

            var plus = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            plus.Text = "+";

            var variableB = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableB.Text = "b";

            var closeParen = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            closeParen.Text = ")";

            var superscript = equation.AddChild(EquationNodeType.Superscript);
            var baseNode = superscript.AddChild(EquationNodeType.Base);
            var baseText = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            baseText.Text = "2";

            try
            {
                // Konvertera ekvationen till MathML
                string mathML = equation.ToMathML();

                // Skriv ut MathML till konsolen
                Console.WriteLine("MathML Output:");
                Console.WriteLine(mathML);

                // Skriv MathML till en cell
                worksheet.Cells["A1"].PutValue("MathML Representation:");
                worksheet.Cells["A2"].PutValue(mathML);
                // Ändrad från worksheet.Cells.AutoFitColumns() till:
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting to MathML: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("EquationToMathMLDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


