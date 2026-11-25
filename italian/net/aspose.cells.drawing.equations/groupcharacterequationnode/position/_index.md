---
title: "GroupCharacterEquationNode.Position"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GroupCharacterEquationNode. Questo attributo specifica la posizione del carattere nell'oggetto"
type: docs
url: /it/net/aspose.cells.drawing.equations/groupcharacterequationnode/position/
---
## GroupCharacterEquationNode.Position property

Questo attributo specifica la posizione del carattere nell'oggetto

```csharp
public EquationCharacterPositionType Position { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il paragrafo dell'equazione e aggiungi un nodo carattere di gruppo
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Imposta la proprietà position (dimostrazione principale)
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Aggiungi testo di base
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";

            // Salva la cartella di lavoro
            string outputPath = "GroupCharacterEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Equation with group character position set to Top has been created successfully.");
        }
    }
}
```

### Vedi anche

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


