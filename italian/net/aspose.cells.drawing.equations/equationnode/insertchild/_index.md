---
title: "EquationNode.InsertChild"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Inserisce un nodo del tipo specificato nella posizione di indice specificata nella lista dei nodi figli del nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/insertchild/
---
## EquationNode.InsertChild method

Inserisce un nodo del tipo specificato nella posizione di indice specificata nell'elenco dei nodi figlio del nodo corrente.

```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | valore indice |
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

    public class EquationNodeMethodInsertChildWithInt32EquationNodeTypDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma di equazione
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Aggiungi il nodo di testo iniziale all'equazione
                var textNode = equationNode.AddChild(EquationNodeType.Text);
                textNode.ToLaTeX(); // Workaround to set text - actual implementation may vary

                // Inserisci un nuovo nodo frazione all'indice 0
                var insertedNode = equationNode.InsertChild(0, EquationNodeType.Fraction);

                Console.WriteLine("InsertChild method executed successfully with index 0 and EquationNodeType.Fraction");
                Console.WriteLine("Inserted node type: " + insertedNode.EquationType);

                // Salva la cartella di lavoro
                workbook.Save("EquationNodeInsertChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertChild method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


