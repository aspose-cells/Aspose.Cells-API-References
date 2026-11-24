---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Ersatzschriftartnamen für einen angegebenen Originalschriftartnamen."
type: docs
url: /de/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Schriftart-Ersatznamen für den angegebenen Originalschriftartnamen.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | String | Originaler Schriftartname. |
| substituteFontNames | String[] | Liste von Ersatzschriftartnamen, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Originaler Schriftartname, der möglicherweise nicht verfügbar ist.
            string originalFontName = "Arial";
            
            // Ersatzschriftartnamen, die verwendet werden, wenn das Original nicht verfügbar ist.
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Rufen Sie die Methode SetFontSubstitutes auf, um Schriftartsubstitutionen zu konfigurieren.
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // Überprüfen Sie die Ersatzschriftarten, indem Sie sie abrufen.
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // Wenden Sie die Schriftart auf eine Zelle an, um die Substitution zu demonstrieren.
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


