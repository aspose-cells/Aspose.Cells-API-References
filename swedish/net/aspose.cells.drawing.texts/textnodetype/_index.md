---
title: "Enum TextNodeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextNodeType enum. Representerar nodtypen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textnodetype/
---
## TextNodeType enumeration

Representerar nodtypen.

```csharp
public enum TextNodeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| TextRun | `0` | Representerar textnoden. |
| TextParagraph | `1` | Representerar textstycket. |
| Equation | `2` | Representerar ekvationstexten. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en textruta och hämta dess textstycken
            int textboxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.TextBody.AppendText("Sample text with ");
            textbox.TextBody.AppendText("different node types");
            
            // Demonstrera användning av TextNodeType
            foreach (TextParagraph paragraph in textbox.TextBody.TextParagraphs)
            {
                foreach (FontSetting portion in paragraph.Children)
                {
                    // Hämta textdelen med StartIndex och Length
                    string portionText = textbox.Text.Substring(portion.StartIndex, portion.Length);
                    Console.WriteLine("Text: " + portionText);
                    Console.WriteLine("Node Type: " + portion.Type.ToString());
                    
                    // Exempel på att kontrollera nodtyp
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

            // Spara resultatet
            workbook.Save("TextNodeTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


