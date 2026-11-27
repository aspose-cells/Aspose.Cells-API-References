---
title: "FractionEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FractionEquationNode‑metod. Bestämmer om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Eftersom FractionEquationNode inte har en parameterlös konstruktor,
                // vi kommer att demonstrera Equals med objekt som förmodligen kommer från någon annanstans i API:et
                // För demonstrationsändamål antar vi att vi har två instanser att jämföra
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Jämför objekten med hjälp av Equals
                bool areEqual = node1.Equals(node2);

                // Visa jämförelsens resultat
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // Jämför med null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Jämför med sig själv
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // Hjälpmetod för att simulera hämtning av FractionEquationNode‑instanser
        // (I verklig användning skulle dessa komma från API:et)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Detta är bara en platshållare – i verkligheten skulle du hämta dessa från API:et
            // Till exempel: worksheet.Equations.AddFractionEquationNode() eller liknande
            return null; // Actual implementation would depend on API
        }
    }
}
```

### Se även

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


