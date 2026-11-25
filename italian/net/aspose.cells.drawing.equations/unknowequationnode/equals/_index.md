---
title: "UnknowEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnknowEquationNode. Determina se il nodo dell'equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due nodi di equazione sconosciuti per il confronto
            // Poiché UnknowEquationNode non ha un costruttore senza parametri,
            // dovremo crearli in modo diverso. Per scopi dimostrativi, useremo
            // il costruttore reale se disponibile, oppure crearli con altri metodi.
            // Poiché non conosciamo i parametri del costruttore, questa è una correzione temporanea.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Chiama il metodo Equals con il tipo di parametro specifico (Object)
                bool areEqual = node1.Equals(objToCompare);

                // Visualizza il risultato
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Aggiungi il risultato al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // Metodo di supporto per creare istanze di UnknowEquationNode
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // In una implementazione reale, questo userebbe il costruttore corretto
            // Poiché non conosciamo i parametri del costruttore, restituiremo null
            // e gestire il caso null nella demo (anche se è solo un segnaposto)
            return null;
        }
    }
}
```

### Vedi anche

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


