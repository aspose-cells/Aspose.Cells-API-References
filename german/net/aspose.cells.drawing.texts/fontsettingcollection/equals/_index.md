---
title: "FontSettingCollection.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Methode."
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object |  |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Setze einen Text
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Erstelle eine weitere FontSettingCollection zum Vergleich
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // Rufe die Equals-Methode auf, um die beiden Sammlungen zu vergleichen
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Ergebnis anzeigen
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


