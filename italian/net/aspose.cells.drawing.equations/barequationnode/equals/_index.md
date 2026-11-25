---
title: "BarEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo BarEquationNode. Determina se il nodo dell'equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due istanze di BarEquationNode per il confronto
            // Nota: La creazione reale di BarEquationNode dipenderebbe dai metodi factory dell'API
            // Per dimostrazione, supporremo che queste siano istanze correttamente inizializzate
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // Confronta node1 con node2 (dovrebbe essere uguale)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // Confronta node1 con node3 (non dovrebbe essere uguale)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // Confronta node1 con null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // Confronta node1 con un tipo di oggetto diverso
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // Metodo di supporto per dimostrare il recupero di un BarEquationNode
        // In un uso reale, dovresti utilizzare il metodo API corretto per crearli
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Questo è solo un segnaposto - l'implementazione reale dipenderebbe dall'API
            // Ad esempio, potrebbe essere creato tramite un oggetto genitore o un metodo factory
            return null; // Replace with actual creation code
        }
    }
}
```

### Vedi anche

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


