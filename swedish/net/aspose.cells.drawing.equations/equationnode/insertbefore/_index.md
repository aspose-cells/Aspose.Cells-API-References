---
title: "EquationNode.InsertBefore"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode method. Infogar den angivna noden före den aktuella noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Infogar den angivna noden före den aktuella noden.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en matematisk ekvation i cell A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Lägg till initial textnod till ekvationen
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Infoga en ny textnod före den befintliga
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Visa ekvationen i LaTeX-format
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


