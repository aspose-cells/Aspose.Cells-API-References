---
title: "TextParagraph.Children"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt alle Textläufe in diesem Absatz zurück. Wenn dieser Absatz leer ist, wird der Absatz selbst zurückgegeben"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Liest alle Textabschnitte in diesem Absatz. Wenn dieser Absatz leer ist, wird der Absatz selbst zurückgegeben.

```csharp
public FontSetting[] Children { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Die Textabsatzsammlung abrufen
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Die Anzahl der Kinder (Textläufe) im Absatz anzeigen
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Die Schriftarteinstellungen jedes Kindes (Textlaufs) ändern
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Eine weitere Zeile mit anderer Formatierung hinzufügen
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Anzeige der aktualisierten Anzahl von Kindern
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Speichere die Arbeitsmappe
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


