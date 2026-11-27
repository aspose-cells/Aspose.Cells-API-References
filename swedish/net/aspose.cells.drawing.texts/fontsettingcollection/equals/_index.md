---
title: "FontSettingCollection.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-metod."
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Ange någon text
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Skapa en annan FontSettingCollection för jämförelse
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // Anropa Equals-metoden för att jämföra de två samlingarna
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Visa resultatet
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Spara arbetsboken
                workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Equals: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


