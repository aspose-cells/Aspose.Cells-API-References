---
title: "EquationNodeParagraph.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNodeParagraph. Determina se il nodo di equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnodeparagraph/equals/
---
## EquationNodeParagraph.Equals method

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

    public class EquationNodeParagraphMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due istanze di EquationNodeParagraph per il confronto
            // Utilizzando il metodo CreateNode per istanziare correttamente i nodi
            EquationNodeParagraph paragraph1 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            EquationNodeParagraph paragraph2 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
            
            // Imposta diversi tipi di giustificazione per renderli disuguali
            paragraph1.Justification = EquationHorizontalJustificationType.Center;
            paragraph2.Justification = EquationHorizontalJustificationType.Left;

            try
            {
                // Chiama il metodo Equals passando paragraph2 come parametro
                bool areEqual = paragraph1.Equals(paragraph2);
                
                // Visualizza il risultato del confronto
                Console.WriteLine($"Are the paragraphs equal? {areEqual}");

                // Crea un altro paragrafo con la stessa giustificazione di paragraph1
                EquationNodeParagraph paragraph3 = EquationNode.CreateNode(EquationNodeType.EquationParagraph, workbook, null) as EquationNodeParagraph;
                paragraph3.Justification = EquationHorizontalJustificationType.Center;

                // Chiama nuovamente Equals con paragraph3
                areEqual = paragraph1.Equals(paragraph3);
                Console.WriteLine($"Are paragraph1 and paragraph3 equal? {areEqual}");

                // Mostra anche il confronto con null
                areEqual = paragraph1.Equals(null);
                Console.WriteLine($"Is paragraph1 equal to null? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro (anche se non sono state apportate modifiche visibili al foglio di lavoro)
            workbook.Save("EquationNodeParagraphEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


