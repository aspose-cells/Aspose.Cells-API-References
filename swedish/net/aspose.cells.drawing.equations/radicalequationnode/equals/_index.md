---
title: "RadicalEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadicalEquationNode‑metod. Bestämmer om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/radicalequationnode/equals/
---
## RadicalEquationNode.Equals method

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

    public class RadicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa två RadicalEquationNode‑instanser
                RadicalEquationNode node1 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));
                RadicalEquationNode node2 = (RadicalEquationNode)Activator.CreateInstance(typeof(RadicalEquationNode));

                // Ställ in olika egenskaper för att demonstrera likhetsjämförelse
                node1.IsDegHide = true;
                node2.IsDegHide = false;

                // Jämför noderna med Equals-metoden
                bool areEqual = node1.Equals(node2);

                // Visa jämförelsens resultat
                Console.WriteLine($"Are nodes equal? {areEqual}");

                // Jämför med samma objekt
                areEqual = node1.Equals(node1);
                Console.WriteLine($"Are node1 and itself equal? {areEqual}");

                // Jämför med null
                areEqual = node1.Equals(null);
                Console.WriteLine($"Are node1 and null equal? {areEqual}");
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

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


