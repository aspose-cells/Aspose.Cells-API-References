---
title: "EquationNode.CreateNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo EquationNode. Crea un nodo del tipo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnode/createnode/
---
## EquationNode.CreateNode method

Crea un nodo del tipo specificato.

```csharp
public static EquationNode CreateNode(EquationNodeType equationType, Workbook workbook, 
    EquationNode parent)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| equationType | EquationNodeType | Tipi di Equation Nodes |
| cartella di lavoro | Cartella di lavoro | L'oggetto workbook associato all'equazione |
| genitore | EquationNode | Il nodo genitore dove si trova questo nodo |

### Valore di ritorno

Se il tipo specificato esiste, viene restituito il nodo corrispondente; se il tipo non esiste, viene restituito un nodo di tipo sconosciuto.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodCreateNodeWithEquationNodeTypeWorkbookEquatiDemo
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
                // Crea un nodo genitore (frazione)
                var fractionNode = EquationNode.CreateNode(EquationNodeType.Fraction, workbook, null);
                
                // Crea i nodi numeratore e denominatore
                var numeratorNode = EquationNode.CreateNode(EquationNodeType.Numerator, workbook, fractionNode);
                var numeratorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, numeratorNode) as TextRunEquationNode;
                numeratorText.Text = "a + b";
                
                var denominatorNode = EquationNode.CreateNode(EquationNodeType.Denominator, workbook, fractionNode);
                var denominatorText = EquationNode.CreateNode(EquationNodeType.Text, workbook, denominatorNode) as TextRunEquationNode;
                denominatorText.Text = "c";

                // Aggiungi la frazione creata all'equazione principale
                equationNode.AddChild(fractionNode);

                Console.WriteLine("Equation created successfully using CreateNode method");
                
                // Visualizza l'equazione in una cella
                worksheet.Cells["A1"].PutValue("Equation Output:");
                worksheet.Cells["B1"].PutValue(equationNode.ToLaTeX());
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CreateNode method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("EquationNodeCreateNodeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [EquationNodeType](../../equationnodetype/)
* class [Workbook](../../../aspose.cells/workbook/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


