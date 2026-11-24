---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GroupCharacterEquationNode-Eigenschaft. Gibt ein Symbolstandard U23DF an. Es wird dringend empfohlen, das Attribut ChrType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können."
type: docs
url: /de/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Gibt ein Symbol an (Standard U+23DF). Es wird dringend empfohlen, das Attribut ChrType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

```csharp
public string GroupChr { get; set; }
```

### Hinweise

Es sollte beachtet werden, dass diese Eigenschaft nur ein Zeichen akzeptiert und bei mehreren übergebenen Zeichen nur das erste Zeichen verwendet wird.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge eine Gleichung zum ersten Arbeitsblatt hinzu
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Den Wurzelknoten der Gleichung abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Erstelle einen Gruppenzeichenknoten mit nach rechts zeigenden Doppelpfeil
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Basistext zum Gruppenzeichen hinzufügen
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // Demonstriere die Verwendung der GroupChr‑Eigenschaft
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Speichere die Arbeitsmappe
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


