---
title: "DelimiterEquationNode.DelimiterShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DelimiterEquationNode-Eigenschaft. Gibt die Form der Trennzeichen im Trennzeichenobjekt an"
type: docs
url: /de/net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

Gibt die Form der Trennzeichen im Trennzeichenobjekt an.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### Beispiele

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

            // Den Gleichungsknoten abrufen
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Erstelle Trennzeichenknoten mit benutzerdefinierter Form
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";

            // Inhalt innerhalb des Trennzeichens hinzufügen
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Content";

            // Speichere die Arbeitsmappe
            workbook.Save("DelimiterShapeDemo.xlsx");

            Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
        }
    }
}
```

### Siehe auch

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


