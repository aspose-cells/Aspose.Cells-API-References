---
title: "BarEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BarEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två BarEquationNode-instansar för jämförelse
            // Obs: Faktisk skapning av BarEquationNode skulle bero på API:s fabriksmetoder
            // För demonstration antar vi att dessa är korrekt initierade instanser
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // Jämför node1 med node2 (ska vara lika)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // Jämför node1 med node3 (ska inte vara lika)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // Jämför node1 med null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // Jämför node1 med en annan objekttyp
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // Hjälpmetod för att demonstrera hämtning av en BarEquationNode
        // I verklig användning skulle du använda rätt API-metod för att skapa dessa
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Detta är bara en platshållare – faktisk implementation skulle bero på API:t
            // Till exempel kan den skapas via ett föräldraobjekt eller en fabriksmetod
            return null; // Replace with actual creation code
        }
    }
}
```

### Se även

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


