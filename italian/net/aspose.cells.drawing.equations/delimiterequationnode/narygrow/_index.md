---
title: "DelimiterEquationNode.NaryGrow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DelimiterEquationNode. Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula"
type: docs
url: /it/net/aspose.cells.drawing.equations/delimiterequationnode/narygrow/
---
## DelimiterEquationNode.NaryGrow property

Specifica se il delimitatore deve espandersi e contrarsi automaticamente con l'altezza della formula.

```csharp
public bool NaryGrow { get; set; }
```

### Osservazioni

Questa proprietà specifica la proprietà di crescita del delimitatore a livello di documento. Quando è disattivata, il delimitatore non crescerà per corrispondere all'altezza del suo componente. Quando è abilitata, il delimitatore cresce verticalmente per corrispondere all'altezza del suo componente.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            var paragraph = textBox.GetEquationParagraph();
            var mathNode = paragraph.GetChild(0);
            
            // Crea un nodo delimitatore con la proprietà NaryGrow
            var delimiterNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Delimiter) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            delimiterNode.DelimiterShape = Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType.Match;
            delimiterNode.NaryGrow = false; // Demonstrating NaryGrow property
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            delimiterNode.SeparatorChar = ",";

            // Aggiungi gli elementi di base
            var baseNode1 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode1 = baseNode1.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode1.Text = "x";

            var baseNode2 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode2 = baseNode2.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode2.Text = "y";

            // Salva e verifica
            string outputFile = "DelimiterEquationNode_NaryGrow_Demo.xlsx";
            workbook.Save(outputFile);

            // Verifica il file salvato
            Workbook verifyWorkbook = new Workbook(outputFile);
            var verifyTextBox = verifyWorkbook.Worksheets[0].Shapes[0] as Aspose.Cells.Drawing.TextBox;
            var verifyNode = verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            
            Console.WriteLine("NaryGrow value: " + verifyNode.NaryGrow); // Should output "False"
        }
    }
}
```

### Vedi anche

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


