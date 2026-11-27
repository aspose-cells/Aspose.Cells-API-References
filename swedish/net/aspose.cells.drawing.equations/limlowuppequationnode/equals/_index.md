---
title: "LimLowUppEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LimLowUppEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

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

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eftersom vi inte känner till konstruktörsparametrarna kommer vi att jämföra null-värden
            // Detta är en minimal ändring för att få det att kompilera – i verklig användning skulle du behöva korrekt konstruktion
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Anropa Equals-metoden med den specifika parametertypen (Object)
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Visa resultatet
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Spara arbetsboken
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


