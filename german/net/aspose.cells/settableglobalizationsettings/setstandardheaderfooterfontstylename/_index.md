---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Setzt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localfontStyleName | String | Lokaler Schriftstilname für Header/Footer. |
| standardName | String | Standardfunktion (en-US Gebietsschema). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie Seiteneinrichtungsoptionen für das Arbeitsblatt
            PageSetup pageSetup = worksheet.PageSetup;

            // Legen Sie einen Header mit etwas Text fest
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Erstellen Sie eine Globalisierungs‑Einstellungsinstanz
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie die Methode SetStandardHeaderFooterFontStyleName auf
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Wenden Sie die Globalisierungseinstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // Der Effekt wird sichtbar sein, wenn das Dokument gerendert oder gedruckt wird
                // Der Schriftsstil "Arial" in Kopf‑/Fußzeilen wird als "Times New Roman" behandelt
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


