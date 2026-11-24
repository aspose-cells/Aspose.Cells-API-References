---
title: "FontSettingCollection.InsertText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection‑Methode. Fügt den Index an der Position ein"
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Fügt den Index an der Position ein.

```csharp
public void InsertText(int index, string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Startindex. |
| Text | String | Der Text. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // Initialen Text festlegen
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Rufe die InsertText‑Methode auf, um Text an Index 7 einzufügen
                fontSettingCollection.InsertText(7, " Inserted");

                // Zeige den modifizierten Text an
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


