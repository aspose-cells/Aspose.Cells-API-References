---
title: "DelimiterEquationNode.EndChar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DelimiterEquationNode-Eigenschaft. Trennzeichen‑Endzeichen"
type: docs
url: /de/net/aspose.cells.drawing.equations/delimiterequationnode/endchar/
---
## DelimiterEquationNode.EndChar property

Endzeichen des Trennzeichens.

```csharp
public string EndChar { get; set; }
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
    public class DelimiterEquationNodePropertyEndCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Den Gleichungsknoten abrufen
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Erstelle einen Trennzeichenknoten mit benutzerdefiniertem Endzeichen
            var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]"; // Demonstrating EndChar property
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;

            // Inhalt innerhalb des Trennzeichens hinzufügen
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";

            // Speichern und überprüfen
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);

            // Überprüfen Sie die gespeicherte Datei
            Workbook verifyWorkbook = new Workbook(outputPath);
            var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
            Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
        }
    }
}
```

### Siehe auch

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


