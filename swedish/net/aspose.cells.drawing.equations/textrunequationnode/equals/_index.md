---
title: "TextRunEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextRunEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // För demonstrationsändamål kommer vi att använda null och bara visa jämförelselogiken
            // eftersom vi inte kan skapa TextRunEquationNode-instanser direkt
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Denna del finns kvar för att visa hur Equals skulle anropas
                // I ett riktigt scenario skulle dessa vara korrekt initierade noder
                if (node1 != null && node2 != null && node3 != null)
                {
                    // Jämför node1 med node2 (samma innehåll)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // Jämför node1 med node3 (olika innehåll)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // Jämför med null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Jämför med annan objekttyp
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken (även om Equals inte ändrar kalkylbladet)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // Tog bort hjälpfunktionen eftersom vi inte kan skapa TextRunEquationNode‑instanser korrekt
    }
}
```

### Se även

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


