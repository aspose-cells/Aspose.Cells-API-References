---
title: "FontSettingCollection.DeleteText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection metod. Ta bort några tecken"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Ta bort vissa tecken.

```csharp
public void DeleteText(int index, int count)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Startindexet. |
| antal | Int32 | Antalet tecken. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
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
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Visa originaltext
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // Anropa DeleteText-metoden för att ta bort 7 tecken med start på index 5
                fontSettingCollection.DeleteText(5, 7);

                // Visa modifierad text
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Spara arbetsboken
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


