---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GroupCharacterEquationNode. Specifica un simbolo predefinito U23DF. Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto."
type: docs
url: /it/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Specifica un simbolo (predefinito U+23DF). Si consiglia vivamente di utilizzare l'attributo ChrType per impostare il carattere di accento. Usa questa impostazione della proprietà se non riesci a trovare il carattere necessario in un tipo noto.

```csharp
public string GroupChr { get; set; }
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
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo radice dell'equazione
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Crea un nodo carattere di gruppo con freccia doppia verso destra
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Aggiungi il testo di base al carattere di gruppo
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // Dimostra l'uso della proprietà GroupChr
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Salva la cartella di lavoro
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


