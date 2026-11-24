---
title: "FontSettingCollection.Format"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Methode. Formatiert den Text mit den Schriftarteinstellungen."
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Formatiere den Text mit FontSetting.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Startindex. |
| Länge | Int32 | Die Länge. |
| Schriftart | Schriftart | Die Schriftart. |
| Flag | StyleFlag | Die Flags der Schriftart. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Initialen Text festlegen
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Erstelle einen Stil und lege seine Schriftarteigenschaften fest
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Erstelle ein Stil-Flag, um anzugeben, welche Schriftarteigenschaften angewendet werden sollen
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // Formatiere Zeichen von Index 7 bis 11 (das Wort "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Arbeitsmappe speichern, um den Effekt zu zeigen
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

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


