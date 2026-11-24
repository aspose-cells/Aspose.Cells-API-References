---
title: "Klasse FontConfigs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontConfigs Klasse. Gibt die Schriftarteinstellungen an"
type: docs
url: /de/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Gibt Schrifteinstellungen an

```csharp
public class FontConfigs
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FontConfigs](fontconfigs/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Liest oder legt den Standard-Schriftartnamen fest. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Gibt an, ob System-Schriftart-Ersatz zuerst verwendet werden soll, wenn eine Schriftart nicht vorhanden ist und kein Ersatz für diese Schriftart festgelegt ist. z. B. unter Ubuntu wird die Schriftart "Arial" normalerweise durch "Liberation Sans" ersetzt. Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Dateninformationen der Schriftdatei abrufen. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Gibt eine Kopie des Arrays zurück, das die Liste der Quellen enthält |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Gibt ein Array zurück, das Schriftart-Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Gibt an, ob die Schriftart verfügbar ist. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Legt den Schriftartenordner fest |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Legt den Schriftartenordner fest |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Legt die Schriftquellen fest. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Schriftart-Ersatznamen für den angegebenen Originalschriftartnamen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Benutzerdefinierten Schriftartenordner festlegen
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieltext mit verschiedenen Schriftarten festlegen
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Benutzerdefinierten Schriftstil anwenden
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Als HTML speichern, um die Schriftartdarstellung zu demonstrieren
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


