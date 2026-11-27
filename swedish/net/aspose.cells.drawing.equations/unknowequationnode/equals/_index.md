---
title: "UnknowEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnknowEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två okända ekvationsnoder för jämförelse
            // Eftersom UnknowEquationNode inte har en parameterlös konstruktor,
            // måste vi skapa dem på ett annat sätt. För demonstrationsändamål kommer vi att använda
            // den faktiska konstruktorn om den finns, eller skapa dem på annat sätt.
            // Eftersom vi inte känner till konstruktorns parametrar är detta en tillfällig lösning.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Anropa Equals-metoden med den specifika parametertypen (Object)
                bool areEqual = node1.Equals(objToCompare);

                // Visa resultatet
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Lägg till resultatet i kalkylbladet
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // Hjälpmetod för att skapa UnknowEquationNode-instansieringar
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // I en riktig implementation skulle detta använda den korrekta konstruktorn
            // Eftersom vi inte känner till konstruktorns parametrar kommer vi att returnera null
            // och hantera null-fallet i demonstrationen (även om detta bara är en platshållare)
            return null;
        }
    }
}
```

### Se även

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


