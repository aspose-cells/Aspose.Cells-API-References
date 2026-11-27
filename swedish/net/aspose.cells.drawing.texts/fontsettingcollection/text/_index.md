---
title: "FontSettingCollection.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-egenskapen. Hämtar och anger texten för formen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/text/
---
## FontSettingCollection.Text property

Hämtar och anger texten för formen.

```csharp
public string Text { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            try
            {
                // Ange ursprunglig text
                fontSettingCollection.Text = "Initial Text Value";
                Console.WriteLine("Initial Text value: " + fontSettingCollection.Text);

                // Ändra texten
                fontSettingCollection.Text = "Modified Text Value";
                Console.WriteLine("Modified Text value: " + fontSettingCollection.Text);

                // Demonstrera hur man lägger till text
                fontSettingCollection.AppendText(" (Appended)");
                Console.WriteLine("After AppendText: " + fontSettingCollection.Text);

                // Spara arbetsboken
                workbook.Save("FontSettingCollectionTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


