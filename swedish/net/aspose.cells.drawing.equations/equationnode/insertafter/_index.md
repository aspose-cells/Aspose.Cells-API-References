---
title: "EquationNode.InsertAfter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode‑metod. Infogar den angivna noden efter den aktuella noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Infogar den angivna noden efter den aktuella noden.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| equationType | EquationNodeType | Typer av Equation‑noder |

### Returvärde

Om den angivna typen finns returneras den motsvarande noden, och om typen inte finns returneras en nod av okänd typ.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en ekvationsform i cell A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Lägg till initial textnod
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Infoga en ny textnod efter den befintliga
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Visa ekvationsstrukturen
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Spara ekvationen i en cell för visuell inspektion
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### Se även

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


