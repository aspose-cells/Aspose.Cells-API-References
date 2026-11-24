---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf‑/Fußzeile gemäß dem angegebenen lokalisierungsspezifischen Schriftstilnamen zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Gibt den standardmäßigen englischen Schriftstilnamen (Regular, Bold, Italic) für Kopf‑/Fußzeile gemäß dem angegebenen lokalisierungsabhängigen Schriftstilnamen zurück.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine benutzerdefinierte Instanz der Globalisierungseinstellungen
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Demonstriere den Methodenaufruf mit Parametertyp (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Wende Globalisierungseinstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Setze die Kopfzeile mit benutzerdefiniertem Schriftstil, der konvertiert wird
                // Verwende die SetHeader‑Methode mit dem Abschnittsparameter (0 = links, 1 = zentriert, 2 = rechts)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Speichere die Arbeitsmappe, um die Wirkung zu zeigen
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Implementierung benutzerdefinierter Globalisierungseinstellungen
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Konvertiere benutzerdefinierte Schriftstilnamen in Standardnamen
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


