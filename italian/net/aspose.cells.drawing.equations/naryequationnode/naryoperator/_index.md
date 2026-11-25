---
title: "NaryEquationNode.NaryOperator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NaryEquationNode. un operatore nary, ad es. È fortemente consigliato utilizzare l'attributo NaryOperatorType per impostare l'operatore nary. Usa questa impostazione di proprietà se non riesci a trovare il carattere necessario in un tipo noto"
type: docs
url: /it/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

un operatore n-ario, ad es. "∑". Si raccomanda vivamente di utilizzare l'attributo NaryOperatorType per impostare l'operatore n-ario. Usa questa impostazione di proprietà se non riesci a trovare il carattere necessario in un tipo conosciuto.

```csharp
public string NaryOperator { get; set; }
```

### Osservazioni

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di equazione
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un nodo operatore n-ario
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Imposta le proprietà dell'operatore n-ario
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Aggiungi pedice (opzionale)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Aggiungi apice (opzionale)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Aggiungi l'espressione di base
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Salva la cartella di lavoro
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### Vedi anche

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


