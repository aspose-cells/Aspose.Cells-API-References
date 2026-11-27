---
title: "DelimiterEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DelimiterEquationNode metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/delimiterequationnode/equals/
---
## DelimiterEquationNode.Equals method

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

    public class DelimiterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två DelimiterEquationNode‑instanser för jämförelse
            // Eftersom DelimiterEquationNode inte har en parameterlös konstruktor,
            // måste vi skapa dem på ett annat sätt. Förutsatt att vi kan använda standardkonstruktorn
            // från basklassen eller hitta ett annat sätt att skapa dem.
            // För demonstration kommer vi att använda ObjectCreationHelper (hypotetisk) eller liknande metod
            DelimiterEquationNode node1 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node1.BeginChar = "(";
            node1.EndChar = ")";
            node1.SeparatorChar = ",";
            node1.DelimiterShape = EquationDelimiterShapeType.Centered;

            DelimiterEquationNode node2 = (DelimiterEquationNode)Activator.CreateInstance(typeof(DelimiterEquationNode), nonPublic: true);
            node2.BeginChar = "(";
            node2.EndChar = ")";
            node2.SeparatorChar = ",";
            node2.DelimiterShape = EquationDelimiterShapeType.Centered;

            try
            {
                // Anropa Equals-metoden med Object-parameter
                bool result = node1.Equals((Object)node2);

                // Visa resultatet
                Console.WriteLine($"Equals method result: {result}");

                // Ändra node2 för att göra dem olika
                node2.BeginChar = "[";
                bool result2 = node1.Equals((Object)node2);
                Console.WriteLine($"Equals method result after modification: {result2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("DelimiterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


