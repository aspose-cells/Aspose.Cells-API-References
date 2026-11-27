---
title: "FontSettingCollection.AppendText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-metod. Lägger till texten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Lägger till texten.

```csharp
public void AppendText(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Ange ursprunglig text
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Anropa AppendText-metoden för att lägga till ytterligare text
                fontSettingCollection.AppendText("World!");

                // Visa den modifierade texten
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Spara arbetsboken
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


