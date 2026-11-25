---
title: "DelimiterEquationNode.EndChar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DelimiterEquationNode. Carattere finale del delimitatore"
type: docs
url: /it/net/aspose.cells.drawing.equations/delimiterequationnode/endchar/
---
## DelimiterEquationNode.EndChar property

Carattere di fine delimitatore.

```csharp
public string EndChar { get; set; }
```

### Osservazioni

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyEndCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo dell'equazione
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un nodo delimitatore con un carattere finale personalizzato
            var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]"; // Demonstrating EndChar property
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;

            // Aggiungi contenuto all'interno del delimitatore
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";

            // Salva e verifica
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Verifica il file salvato
            Workbook verifyWorkbook = new Workbook(outputPath);
            var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
            Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
        }
    }
}
```

### Vedi anche

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


