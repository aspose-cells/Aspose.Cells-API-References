---
title: "BorderBoxEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BorderBoxEquationNode-metod. Avgör om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa två BorderBoxEquationNode‑instanser för jämförelse
                // Eftersom BorderBoxEquationNode inte har en parameterlös konstruktor,
                // kommer vi att använda basklassens konstruktor (förutsatt att EquationNode har en sådan)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Jämför noderna med Equals-metoden
                bool areEqual = node1.Equals((object)node2);
                
                // Visa jämförelsens resultat
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Jämför med en annan objekttyp
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


