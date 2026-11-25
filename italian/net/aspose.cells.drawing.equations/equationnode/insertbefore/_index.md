---
title: "EquationNode.InsertBefore"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Inserisce il nodo specificato prima del nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/insertbefore/
---
## EquationNode.InsertBefore method

Inserisce il nodo specificato prima del nodo corrente.

```csharp
public EquationNode InsertBefore(EquationNodeType equationType)
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

    public class EquationNodeMethodInsertBeforeWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'equazione matematica nella cella A1
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            // Aggiungi il nodo di testo iniziale all'equazione
            var textNode = equationNode.AddChild(EquationNodeType.Text);
            textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

            try
            {
                // Inserisci un nuovo nodo di testo prima di quello esistente
                var insertedNode = equationNode.InsertBefore(EquationNodeType.Text);
                insertedNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                Console.WriteLine("InsertBefore method executed successfully with EquationNodeType.Text parameter");
                
                // Visualizza l'equazione in formato LaTeX
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertBefore method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("EquationNodeInsertBeforeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


