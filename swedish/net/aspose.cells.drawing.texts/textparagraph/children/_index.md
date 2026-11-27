---
title: "TextParagraph.Children"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar alla textrader i detta stycke. Om detta stycke är tomt returneras stycket självt"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Hämtar alla textkörningar i denna paragraf. Om paragrafen är tom, returneras paragrafen själv.

```csharp
public FontSetting[] Children { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Hämta samlingen av textstycken
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Visa antalet underobjekt (textrader) i stycket
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Ändra teckensnittsinställningarna för varje underobjekt (textrad)
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Lägg till en annan rad med annan formatering
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Visa det uppdaterade antalet barn
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Spara arbetsboken
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


