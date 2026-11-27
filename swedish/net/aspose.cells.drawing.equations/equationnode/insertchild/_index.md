---
title: "EquationNode.InsertChild"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode‑metod. Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens lista med barnnoder"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens lista över barnnoder.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexvärde |
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

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
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
                // Lägg till initial textnod till ekvationen
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Infoga en ny bråknod vid index 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Spara arbetsboken
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


