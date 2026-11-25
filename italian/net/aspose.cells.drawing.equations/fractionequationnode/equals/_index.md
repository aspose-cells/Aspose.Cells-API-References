---
title: "FractionEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FractionEquationNode. Determina se il nodo di equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Poiché FractionEquationNode non ha un costruttore senza parametri,
                // dimostreremo Equals con oggetti che presumibilmente provengono da altre parti dell'API
                // Ai fini della dimostrazione, supponiamo di avere due istanze da confrontare
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Confronta gli oggetti usando Equals
                bool areEqual = node1.Equals(node2);

                // Visualizza il risultato del confronto
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // Confronta con null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Confronta con se stesso
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // Metodo di supporto per simulare l'ottenimento di istanze FractionEquationNode
        // (In un utilizzo reale, questi provengono dall'API)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Questo è solo un segnaposto - in realtà otterresti questi dall'API
            // Ad esempio: worksheet.Equations.AddFractionEquationNode() o simile
            return null; // Actual implementation would depend on API
        }
    }
}
```

### Vedi anche

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


