---
title: "FontSettingCollection.Replace"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Methode. Ersetzt den Text."
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Ersetzt den Text.

```csharp
public void Replace(int index, int count, string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Startindex. |
| Anzahl | Int32 | Die Anzahl der Zeichen. |
| Text | String | Der Text. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Rufen Sie die Replace-Methode auf, um 8 Zeichen ab Index 9 durch neuen Text zu ersetzen.
                fontSettingCollection.Replace(9, 8, "replaced");

                // Zeige den modifizierten Text an
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Speichere die Arbeitsmappe
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Ersetzt den Text.

```csharp
public void Replace(string oldValue, string newValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | String | Der alte Text. |
| newValue | String | Der neue Text. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine Form hinzu und setzen Sie den Text.
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Ersetzen Sie den Text in der Form.
            shape.TextBody.Replace("３４", "ABC");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


