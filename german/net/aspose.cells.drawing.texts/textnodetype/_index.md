---
title: "Enum TextNodeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextNodeType enum. Stellt den Knotentyp dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textnodetype/
---
## TextNodeType enumeration

Stellt den Knotentyp dar.

```csharp
public enum TextNodeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| TextRun | `0` | Stellt den Textknoten dar. |
| TextParagraph | `1` | Stellt den Textabsatz dar. |
| Equation | `2` | Stellt den Gleichungstext dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextNodeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Textfeld und erhalte seine Textabsätze
            int textboxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.TextBody.AppendText("Sample text with ");
            textbox.TextBody.AppendText("different node types");
            
            // Demonstriere die Verwendung von TextNodeType
            foreach (TextParagraph paragraph in textbox.TextBody.TextParagraphs)
            {
                foreach (FontSetting portion in paragraph.Children)
                {
                    // Hole den Textabschnitt mit StartIndex und Length
                    string portionText = textbox.Text.Substring(portion.StartIndex, portion.Length);
                    Console.WriteLine("Text: " + portionText);
                    Console.WriteLine("Node Type: " + portion.Type.ToString());
                    
                    // Beispiel für die Überprüfung des Knotentyps
                    if (portion.Type == TextNodeType.TextRun)
                    {
                        portion.Font.Color = System.Drawing.Color.Red;
                    }
                    else if (portion.Type == TextNodeType.Equation)
                    {
                        portion.Font.Color = System.Drawing.Color.Blue;
                    }
                }
            }

            // Ergebnis speichern
            workbook.Save("TextNodeTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


