---
title: "MatrixEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo MatrixEquationNode. Determina se il nodo equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/matrixequationnode/equals/
---
## MatrixEquationNode.Equals method

Determina se il nodo dell'equazione corrente è uguale al nodo specificato

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | Il nodo specificato |

### Esempi

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
                // Poiché MatrixEquationNode non ha un costruttore senza parametri,
                // dimostreremo il metodo Equals usando un approccio diverso
                Console.WriteLine("MatrixEquationNode Equals demonstration:");
                
                // Nota: L'instanziazione reale richiederebbe parametri di costruttore appropriati
                // Questo serve solo a mostrare il modello di utilizzo del metodo Equals
                MatrixEquationNode node1 = null; // Would normally be created with proper constructor
                MatrixEquationNode node2 = null; // Would normally be created with proper constructor

                if (node1 != null && node2 != null)
                {
                    // Confronta i nodi usando il metodo Equals
                    bool areEqual = node1.Equals(node2);
                    Console.WriteLine($"Are the matrix equation nodes equal? {areEqual}");

                    // Confronta un nodo con se stesso
                    bool selfEqual = node1.Equals(node1);
                    Console.WriteLine($"Is node1 equal to itself? {selfEqual}");
                }

                // Confronta con null
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

### Vedi anche

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


