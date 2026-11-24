---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Methode. Legt die Schriftordner fest"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Legt die Schriftordner fest

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Bereite das Array der Schriftordner vor
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Rufen Sie die Methode SetFontFolders mit String[]- und Boolean-Parametern auf.
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Demonstriere den Effekt durch die Verwendung einer benutzerdefinierten Schrift
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


