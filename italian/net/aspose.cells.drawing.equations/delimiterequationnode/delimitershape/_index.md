---
title: "DelimiterEquationNode.DelimiterShape"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DelimiterEquationNode. Specifica la forma dei delimitatori nell'oggetto delimitatore"
type: docs
url: /it/net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

Specifica la forma dei delimitatori nell'oggetto delimitatore.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyDelimiterShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo dell'equazione
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un nodo delimitatore con forma personalizzata
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";

            // Aggiungi contenuto all'interno del delimitatore
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Content";

            // Salva la cartella di lavoro
            workbook.Save("DelimiterShapeDemo.xlsx");

            Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
        }
    }
}
```

### Vedi anche

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


