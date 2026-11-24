---
title: "FontSettingCollection.DeleteText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Methode. Löscht einige Zeichen."
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Löscht einige Zeichen.

```csharp
public void DeleteText(int index, int count)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Startindex. |
| Anzahl | Int32 | Die Anzahl der Zeichen. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Initialen Text festlegen
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Originalen Text anzeigen.
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // Rufen Sie die DeleteText-Methode auf, um 7 Zeichen ab Index 5 zu entfernen.
                fontSettingCollection.DeleteText(5, 7);

                // Geänderten Text anzeigen.
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


