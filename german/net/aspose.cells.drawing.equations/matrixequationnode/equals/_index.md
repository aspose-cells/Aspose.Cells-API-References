---
title: "MatrixEquationNode.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MatrixEquationNode-Methode. Bestimmen Sie, ob der aktuelle Gleichungsknoten dem angegebenen Knoten entspricht"
type: docs
url: /de/net/aspose.cells.drawing.equations/matrixequationnode/equals/
---
## MatrixEquationNode.Equals method

Bestimme, ob der aktuelle Gleichungsknoten dem angegebenen Knoten gleich ist

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Der angegebene Knoten |

### Beispiele

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
                // Da MatrixEquationNode keinen parameterlosen Konstruktor hat,
                // Wir demonstrieren die Equals-Methode mit einem anderen Ansatz
                Console.WriteLine("MatrixEquationNode Equals demonstration:");
                
                // Hinweis: Eine tatsächliche Instanziierung würde korrekte Konstruktorparameter erfordern
                // Dies dient lediglich dazu, das Verwendungsmuster der Equals-Methode zu zeigen
                MatrixEquationNode node1 = null; // Would normally be created with proper constructor
                MatrixEquationNode node2 = null; // Would normally be created with proper constructor

                if (node1 != null && node2 != null)
                {
                    // Vergleichen Sie die Knoten mit der Equals-Methode
                    bool areEqual = node1.Equals(node2);
                    Console.WriteLine($"Are the matrix equation nodes equal? {areEqual}");

                    // Vergleiche einen Knoten mit sich selbst
                    bool selfEqual = node1.Equals(node1);
                    Console.WriteLine($"Is node1 equal to itself? {selfEqual}");
                }

                // Vergleiche mit null
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

### Siehe auch

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


