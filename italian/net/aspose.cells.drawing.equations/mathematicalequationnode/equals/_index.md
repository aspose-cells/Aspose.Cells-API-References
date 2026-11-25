---
title: "MathematicalEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo MathematicalEquationNode. Determina se il nodo dell'equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Crea due istanze di MathematicalEquationNode per il confronto
                // Poiché MathematicalEquationNode non ha un costruttore senza parametri,
                // dovremo passare null o parametri appropriati
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Confronta i nodi usando il metodo Equals
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Visualizza il risultato del confronto
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Confronta con un tipo di oggetto diverso
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


