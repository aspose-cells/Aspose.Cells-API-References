---
title: "DelimiterEquationNode.BeginChar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DelimiterEquationNode-Eigenschaft. Trennzeichen‑Anfangszeichen"
type: docs
url: /de/net/aspose.cells.drawing.equations/delimiterequationnode/beginchar/
---
## DelimiterEquationNode.BeginChar property

Anfangszeichen des Trennzeichens.

```csharp
public string BeginChar { get; set; }
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
    public class DelimiterEquationNodePropertyBeginCharDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge eine Gleichung zum ersten Arbeitsblatt hinzu
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // Den Wurzelknoten der Gleichung abrufen
            var mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Füge einen Trennzeichenknoten mit benutzerdefinierten Anfangs‑/Endzeichen hinzu
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.BeginChar = "#";
            delimiterNode.EndChar = "*";
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            
            // Inhalt innerhalb des Trennzeichens hinzufügen
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Content";
            
            // Speichere die Arbeitsmappe
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
        }
    }
}
```

### Siehe auch

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


