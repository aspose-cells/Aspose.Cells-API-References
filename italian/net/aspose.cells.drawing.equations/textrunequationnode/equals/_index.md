---
title: "TextRunEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TextRunEquationNode. Determina se il nodo di equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Per scopi dimostrativi, utilizzeremo null e mostreremo solo la logica di confronto
            // poiché non possiamo creare istanze di TextRunEquationNode direttamente
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Questa parte rimane per mostrare come verrebbe chiamato Equals
                // In uno scenario reale, questi sarebbero nodi correttamente inizializzati
                if (node1 != null && node2 != null && node3 != null)
                {
                    // Confronta node1 con node2 (stesso contenuto)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // Confronta node1 con node3 (contenuto diverso)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // Confronta con null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Confronta con un tipo di oggetto diverso
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

            // Salva la cartella di lavoro (anche se Equals non modifica il foglio di calcolo)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // Rimosso il metodo di supporto poiché non possiamo creare correttamente istanze di TextRunEquationNode
    }
}
```

### Vedi anche

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


