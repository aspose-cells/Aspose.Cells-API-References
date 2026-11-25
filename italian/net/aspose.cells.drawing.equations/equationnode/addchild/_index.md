---
title: "EquationNode.AddChild"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Inserisce un nodo del tipo specificato alla fine dell'elenco dei nodi figli del nodo corrente"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Inserisci un nodo del tipo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | EquationNodeType | Tipi di Equation Nodes |

### Valore di ritorno

Se il tipo specificato esiste, viene restituito il nodo corrispondente; se il tipo non esiste, viene restituito un nodo di tipo sconosciuto.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationNodeMethodAddChildWithEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo radice della matematica
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un nodo funzione e aggiungi i figli
            FunctionEquationNode functionNode = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
            
            // Aggiungi nome della funzione con apice
            EquationNode functionName = functionNode.AddChild(EquationNodeType.FunctionName);
            EquationNode supNode = functionName.AddChild(EquationNodeType.Sup);
            
            // Aggiungi testo di base per il nome della funzione
            EquationNode baseNode = supNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "Add";
            
            // Aggiungi testo in apice
            EquationNode superscriptNode = supNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscriptNode.AddChild(EquationNodeType.Text);
            superscriptText.Text = "-2";
            
            // Aggiungi argomento della funzione
            EquationNode argumentNode = functionNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode argumentText = (TextRunEquationNode)argumentNode.AddChild(EquationNodeType.Text);
            argumentText.Text = "x";

            // Salva la cartella di lavoro
            workbook.Save("EquationNodeAddChildDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Inserisce il nodo specificato alla fine dell'elenco dei nodi figlio del nodo corrente.

```csharp
public void AddChild(EquationNode node)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nodo | EquationNode | Il nodo specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodAddChildWithEquationNodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma di equazione
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);
            var equationNode = shape.GetEquationParagraph();

            try
            {
                // Crea un nodo di testo da utilizzare come genitore
                var parentNode = equationNode.AddChild(EquationNodeType.Text);
                if (parentNode is TextRunEquationNode textNode)
                {
                    textNode.Text = "Parent Text";
                }

                // Crea un nodo figlio da aggiungere usando il metodo statico CreateNode
                var childNode = EquationNode.CreateNode(EquationNodeType.Text, workbook, null);
                if (childNode is TextRunEquationNode childTextNode)
                {
                    childTextNode.Text = "Child Text";
                }

                // Chiama il metodo AddChild con parametro EquationNode
                parentNode.AddChild(childNode);

                Console.WriteLine("AddChild method called successfully with EquationNode parameter");
                Console.WriteLine("Parent node has children: " + (parentNode.GetChild(0) != null));

                // Salva la cartella di lavoro
                workbook.Save("EquationNodeAddChildDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling AddChild: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


