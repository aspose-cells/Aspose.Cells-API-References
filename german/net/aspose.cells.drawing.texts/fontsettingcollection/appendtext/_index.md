---
title: "FontSettingCollection.AppendText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Methode. Fügt den Text an"
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Fügt den Text an.

```csharp
public void AppendText(string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Initialen Text festlegen
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Rufe die AppendText-Methode auf, um zusätzlichen Text anzufügen
                fontSettingCollection.AppendText("World!");

                // Zeige den modifizierten Text an
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


