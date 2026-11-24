---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Methode. Legt den Schriftordner fest"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Legt den Schriftartenordner fest

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolder | String | Der Ordner, der TrueType-Schriften enthält. |
| rekursiv | Boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Gib den Pfad des Schriftordners und an, ob rekursiv gesucht werden soll
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Rufe SetFontFolder mit den angegebenen Parametern auf
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Erstelle ein Arbeitsbuch, um die Schriftverwendung zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Setze einen Stil, der möglicherweise Schriften aus dem angegebenen Ordner verwendet
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Speichere die Arbeitsmappe
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


