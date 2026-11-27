---
title: "FontSettingCollection.Format"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection metod. Formatera texten med teckensnittinställning"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Formatera texten med font‑inställning.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Startindexet. |
| length | Int32 | Längden. |
| teckensnitt | Teckensnitt | Teckensnittet. |
| flagga | StyleFlag | Flaggorna för teckensnittet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Skapa en stil och ange dess teckensnittsegenskaper
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Skapa stilflagga för att ange vilka teckensnittsegenskaper som ska tillämpas
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // Formatera tecken från index 7 till 11 (ordet "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Spara arbetsboken för att visa effekten
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


