---
title: "FontConfigs.SetFontFolders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Legt den Schriftordner fest"
type: docs
url: /de/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Legt den Schriftartenordner fest

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | String[] | Die Ordner, die TrueType-Schriftarten enthalten. |
| rekursiv | Boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Legen Sie einen Text fest, der benutzerdefinierte Schriftarten verwendet.
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Bereiten Sie Schriftordner vor (ersetzen Sie sie durch tatsächliche Pfade auf Ihrem System).
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // Rufen Sie die Methode SetFontFolders mit String[]- und Boolean-Parametern auf.
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Wenden Sie eine Schriftart an, die sich möglicherweise in einem dieser Ordner befindet.
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


