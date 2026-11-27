---
title: "FontSettingCollection.Replace"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection metod. Ersätt texten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Ersätt texten.

```csharp
public void Replace(int index, int count, string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Startindexet. |
| antal | Int32 | Antalet tecken. |
| text | String | Texten. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Ange ursprunglig text
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Anropa Replace-metoden för att ersätta 8 tecken med start på index 9 med ny text
                fontSettingCollection.Replace(9, 8, "replaced");

                // Visa den modifierade texten
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Spara arbetsboken
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

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Ersätt texten.

```csharp
public void Replace(string oldValue, string newValue)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldValue | String | Den gamla texten. |
| nyttVärde | String | Den nya texten. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en form och ange text
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Ersätt text i formen
            shape.TextBody.Replace("３４", "ABC");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


