---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Methode. Legt Ersatzschriftartnamen für einen angegebenen Originalschriftartnamen fest"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Legt Schriftart-Ersatznamen für einen gegebenen Originalschriftartnamen fest.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Originaler Schriftartname und seine Ersatzschriften
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Rufen Sie SetFontSubstitutes mit den angegebenen Parametern auf
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Erstelle eine Arbeitsmappe, um den Effekt zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Stil mit Originalschriftart festlegen
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Speichere die Arbeitsmappe
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


