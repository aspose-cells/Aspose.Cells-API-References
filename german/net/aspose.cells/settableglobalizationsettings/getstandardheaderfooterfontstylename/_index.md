---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den standardmäßigen englischen Schriftstilnamen Regular Bold Italic für Kopf-/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen zurück"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Gibt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf‑/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen zurück.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localfontStyleName | String | Lokaler Schriftstilname für Header/Footer. |

### Rückgabewert

Standardenglischer Schriftstilname (Regular, Bold, Italic)

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Legen Sie eine Standardzuordnung für den Schriftstilnamen von Header/Footer fest
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Wenden Sie die Einstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Rufen Sie die Methode GetStandardHeaderFooterFontStyleName mit einem lokalen Schriftstilnamen auf
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Ergebnis anzeigen
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Erstellen Sie einen Header mit dem lokalen Schriftstilnamen
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Zeigen Sie die Wirkung in der Tabellenkalkulation
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


