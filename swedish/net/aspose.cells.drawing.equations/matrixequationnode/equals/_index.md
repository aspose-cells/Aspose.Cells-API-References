---
title: "MatrixEquationNode.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MatrixEquationNode-metod. Bestäm om den aktuella ekvationsnoden är lika med den angivna noden"
type: docs
url: /sv/net/aspose.cells.drawing.equations/matrixequationnode/equals/
---
## MatrixEquationNode.Equals method

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

    public class MatrixEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Eftersom MatrixEquationNode inte har en parameterlös konstruktor,
                // kommer vi att demonstrera Equals-metoden med ett annat tillvägagångssätt
                Console.WriteLine("MatrixEquationNode Equals demonstration:");
                
                // Obs: Verklig instansiering skulle kräva korrekta konstruktörsparametrar
                // Detta är bara för att visa användningsmönstret för Equals-metoden
                MatrixEquationNode node1 = null; // Would normally be created with proper constructor
                MatrixEquationNode node2 = null; // Would normally be created with proper constructor

                if (node1 != null && node2 != null)
                {
                    // Jämför noderna med Equals-metoden
                    bool areEqual = node1.Equals(node2);
                    Console.WriteLine($"Are the matrix equation nodes equal? {areEqual}");

                    // Jämför en nod med sig själv
                    bool selfEqual = node1.Equals(node1);
                    Console.WriteLine($"Is node1 equal to itself? {selfEqual}");
                }

                // Jämför med null
                if (node1 != null)
                {
                    bool nullEqual = node1.Equals(null);
                    Console.WriteLine($"Is node1 equal to null? {nullEqual}");
                }
                else
                {
                    Console.WriteLine("Node1 is null - cannot demonstrate Equals method");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MatrixEquationNode Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


