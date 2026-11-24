---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Methode. Gibt ein Array zurück, das Ersatzschriftartnamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Gibt ein Array zurück, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Rückgabewert

Ein Array, das Schriftart‑Ersetzungsnamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Erstelle individuelle Schriftkonfigurationen
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Setzen Sie Schriftart-Ersatz für "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Abrufen von Schriftart-Ersatz für "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Erstelle eine Arbeitsmappe, um den Effekt zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Stil mit Originalschriftart festlegen
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Speichere die Arbeitsmappe
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


