---
title: "EquationNode.CreateNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode method. Skapa en nod av den angivna typen"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Skapa en nod av den angivna typen.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | EquationNodeType | Typer av Equation‑noder |
| arbetsbok | Arbetsbok | Arbetsboksobjektet som är associerat med ekvationen |
| förälder | EquationNode | Den föräldraknuten där denna nod är placerad |

### Returvärde

Om den angivna typen finns returneras den motsvarande noden, och om typen inte finns returneras en nod av okänd typ.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en ekvationsform
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Skapa en föräldraknut (bråk)
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Skapa noder för täljare och nämnare
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Lägg till det skapade bråket i huvudekvationen
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Visa ekvationen i en cell
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


