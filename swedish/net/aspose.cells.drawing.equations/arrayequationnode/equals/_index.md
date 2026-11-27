---
title: "ArrayEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ArrayEquationNode‑metod. Bestämmer om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/arrayequationnode/equals/
---
## ArrayEquationNode.Equals method

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

    public class ArrayEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två array‑ekvationsnoder
            ArrayEquationNode arrayEquation1 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
            ArrayEquationNode arrayEquation2 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);

            // Lägg till barnnoder för att göra dem olika
            EquationNode child1 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation1);
            // Använd ToLaTeX() eller ToMathML() istället för Value‑egenskapen
            arrayEquation1.AddChild(child1);

            EquationNode child2 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation2);
            arrayEquation2.AddChild(child2);

            try
            {
                // Anropa Equals‑metoden med olika objekt
                bool result1 = arrayEquation1.Equals(arrayEquation2);
                Console.WriteLine($"Comparing different array equations: {result1}");

                // Anropa Equals med samma objekt
                bool result2 = arrayEquation1.Equals(arrayEquation1);
                Console.WriteLine($"Comparing same array equation: {result2}");

                // Anropa Equals med null
                bool result4 = arrayEquation1.Equals(null);
                Console.WriteLine($"Comparing with null: {result4}");
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("ArrayEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ArrayEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


