---
title: "BorderBoxEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo BorderBoxEquationNode. Determina se il nodo equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Crea due istanze di BorderBoxEquationNode per il confronto
                // Poiché BorderBoxEquationNode non ha un costruttore senza parametri,
                // useremo il costruttore della classe base (supponendo che EquationNode ne abbia uno)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Confronta i nodi usando il metodo Equals
                bool areEqual = node1.Equals((object)node2);
                
                // Visualizza il risultato del confronto
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Confronta con un tipo di oggetto diverso
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


