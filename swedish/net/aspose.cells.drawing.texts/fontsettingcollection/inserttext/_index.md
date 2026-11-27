---
title: "FontSettingCollection.InsertText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-metod. Infogar index på positionen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Infoga indexet på positionen.

```csharp
public void InsertText(int index, string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Startindexet. |
| text | String | Texten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // Ange ursprunglig text
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Anropa InsertText-metoden för att infoga text vid index 7
                fontSettingCollection.InsertText(7, " Inserted");

                // Visa den modifierade texten
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Spara arbetsboken
                workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertText method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


