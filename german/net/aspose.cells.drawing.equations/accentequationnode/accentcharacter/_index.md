---
title: "AccentEquationNode.AccentCharacter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AccentEquationNode-Eigenschaft. Dieses Attribut gibt den Typ des kombinierten diakritischen Zeichens an, das an die Basis der Akzentfunktion angehängt wird. Das Standardakzentzeichen ist U0302. Es wird dringend empfohlen, das Attribut AccentType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können."
type: docs
url: /de/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Dieses Attribut gibt den Typ des kombinierenden diakritischen Zeichens an, das an die Basis der Akzentfunktion angehängt wird. Das Standard-Akzentzeichen ist U+0302. Es wird dringend empfohlen, das Attribut AccentType zu verwenden, um das Akzentzeichen festzulegen. Verwenden Sie diese Eigenschaftseinstellung, wenn Sie das benötigte Zeichen in einem bekannten Typ nicht finden können.

```csharp
public string AccentCharacter { get; set; }
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
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie dem ersten Arbeitsblatt eine Gleichungsform hinzu.
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hole den Gleichungsknoten und füge einen Akzentknoten hinzu
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Setze das Akzentzeichen (in diesem Fall das Zirkumflex)
            accentNode.AccentCharacter = "\u0302";

            // Füge Basistext für den Akzent hinzu
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Speichere die Arbeitsmappe
            workbook.Save("AccentEquationDemo.xlsx");

            // Verifiziere die gespeicherte Datei, indem du sie erneut lädst
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Gib das Akzentzeichen aus, um die Eigenschaft zu demonstrieren
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### Siehe auch

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


