---
title: "EquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnode/equals/
---
## EquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två ekvationsnoder för jämförelse
            EquationNode node1 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            EquationNode node2 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

            try
            {
                // Anropa Equals-metoden med Object-parameter
                bool areEqual = node1.Equals((object)node2);

                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Ändra node2 för att göra dem olika
                node2.AddChild(EquationNodeType.Base);

                areEqual = node1.Equals((object)node2);
                Console.WriteLine($"After modification, are they equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            workbook.Save("EquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


