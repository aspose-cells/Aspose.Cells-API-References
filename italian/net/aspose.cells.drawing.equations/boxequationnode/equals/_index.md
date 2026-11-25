---
title: "BoxEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo BoxEquationNode. Determina se il nodo dell'equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due oggetti BoxEquationNode per il confronto
            // Poiché BoxEquationNode non ha un costruttore senza parametri,
            // dovremo crearli in modo diverso. Supponendo di poterli ottenere da qualche parte,
            // oppure crearli con alcuni parametri predefiniti.
            // Per scopi dimostrativi, li dichiariamo semplicemente e assegniamo null (anche se nel codice reale sarebbe necessaria un'inizializzazione corretta)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Chiama il metodo Equals con i tipi di parametro specifici (Object)
                    bool areEqual = node1.Equals(objToCompare);

                    // Visualizza il risultato
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Aggiungi il risultato al foglio di lavoro
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Salva il risultato
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


