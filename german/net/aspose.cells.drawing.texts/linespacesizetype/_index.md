---
title: "Enum LineSpaceSizeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Stellt den Einheitstyp der Zeilenabstandgröße dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Stellt den Einheitstyp der Zeilenabstandgröße dar.

```csharp
public enum LineSpaceSizeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Percentage | `0` | Stellt in Einheiten eines Prozentsatzes der Textgröße dar. |
| Points | `1` | Stellt in Einheiten von Punkten dar. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine Textfeldform hinzu
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Legen Sie den Textinhalt fest
            textBox.Text = "Sample Text\nSecond Line";
            
            // Greifen Sie auf den ersten Absatz des Textfelds zu
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Setzen Sie den Nachlaufgrößentyp auf Punkte
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Setzen Sie den Nachlaufwert (12 Punkte)
            paragraph.SpaceAfter = 12;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


