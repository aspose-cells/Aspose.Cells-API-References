---
title: "MathematicalEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MathematicalEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa två instanser av MathematicalEquationNode för jämförelse
                // Eftersom MathematicalEquationNode inte har en parameterlös konstruktor,
                // vi måste skicka null eller lämpliga parametrar
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Jämför noderna med Equals-metoden
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Visa jämförelsens resultat
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Jämför med en annan objekttyp
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


