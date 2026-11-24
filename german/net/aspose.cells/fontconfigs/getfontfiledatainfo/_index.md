---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Dateninformationen der Schriftdatei abrufen"
type: docs
url: /de/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Dateninformationen der Schriftdatei abrufen.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontName | String | Schriftname |
| isBold | Boolean | Der Schriftstil ist fett oder nicht |
| isItalic | Boolean | Der Schriftstil ist kursiv oder nicht |
| isExactStyle | Boolean | Ob der angegebene fett/kursiv-Stil exakt übereinstimmt |

### Rückgabewert

Dateninformationen der Schriftdatei.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Rufen Sie GetFontFileDataInfo mit spezifischen Parametern auf (geändert zu statischem Aufruf)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Informationen über die Schriftdatei anzeigen
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Effekt in einer Arbeitsmappe demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Stil mit der geprüften Schrift festlegen
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Stil auf eine Zelle anwenden
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Speichere die Arbeitsmappe
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


