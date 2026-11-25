---
title: "EquationNode.InsertAfter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Inserisce il nodo specificato dopo il nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/insertafter/
---
## EquationNode.InsertAfter method

Inserisce il nodo specificato dopo il nodo corrente.

```csharp
public EquationNode InsertAfter(EquationNodeType equationType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | EquationNodeType | Tipi di Equation Nodes |

### Valore di ritorno

Se il tipo specificato esiste, viene restituito il nodo corrispondente; se il tipo non esiste, viene restituito un nodo di tipo sconosciuto.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodInsertAfterWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma di equazione nella cella A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Aggiungi il nodo di testo iniziale
            var firstNode = equationNode.AddChild(EquationNodeType.Text);
            if (firstNode is TextRunEquationNode textNode)
            {
                textNode.Text = "Initial Text";
            }

            try
            {
                // Inserisci un nuovo nodo di testo dopo quello esistente
                var insertedNode = equationNode.InsertAfter(EquationNodeType.Text);
                if (insertedNode is TextRunEquationNode insertedTextNode)
                {
                    insertedTextNode.Text = "Inserted After";
                }

                Console.WriteLine("InsertAfter method executed successfully with EquationNodeType.Text parameter");
                
                // Visualizza la struttura dell'equazione
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                
                // Salva l'equazione in una cella per l'ispezione visiva
                worksheet.Cells["A2"].PutValue("Equation Output:");
                worksheet.Cells["B2"].PutValue(equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertAfter method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("EquationNodeInsertAfterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


