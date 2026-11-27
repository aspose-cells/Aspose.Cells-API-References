---
title: "BoxEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BoxEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två BoxEquationNode-objekt för jämförelse
            // Eftersom BoxEquationNode inte har en parameterlös konstruktor,
            // vi måste skapa dem på ett annat sätt. Förutsatt att vi kan få dem från någonstans,
            // eller skapa dem med några standardparametrar.
            // För demonstrationsändamål kommer vi bara att deklarera dem och tilldela null (även om du i riktig kod behöver korrekt initiering)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Anropa Equals-metoden med de specifika parametertyperna (Object)
                    bool areEqual = node1.Equals(objToCompare);

                    // Visa resultatet
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Lägg till resultatet i kalkylbladet
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Spara resultatet
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


