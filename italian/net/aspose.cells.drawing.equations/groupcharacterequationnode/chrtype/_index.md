---
title: "GroupCharacterEquationNode.ChrType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GroupCharacterEquationNode. Specifica i caratteri combinanti per valore di tipo"
type: docs
url: /it/net/aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/
---
## GroupCharacterEquationNode.ChrType property

Specifica i caratteri combinanti per valore di tipo.

```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyChrTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo radice dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Aggiungi un nodo carattere di gruppo
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Imposta le proprietà del carattere di gruppo
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Aggiungi testo di base
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "test";

            // Salva la cartella di lavoro
            workbook.Save("GroupCharacterEquationDemo.xlsx");

            // Verifica il file salvato
            Workbook verifyWorkbook = new Workbook("GroupCharacterEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            GroupCharacterEquationNode verifyNode = (GroupCharacterEquationNode)verifyTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);

            Console.WriteLine("Group Character Type: " + verifyNode.ChrType);
            Console.WriteLine("Group Character: " + verifyNode.GroupChr);
            Console.WriteLine("Base Text: " + ((TextRunEquationNode)verifyNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### Vedi anche

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


