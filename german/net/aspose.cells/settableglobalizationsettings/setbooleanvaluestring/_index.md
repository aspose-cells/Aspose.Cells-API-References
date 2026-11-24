---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt den Anzeigestringwert für den booleschen Zellwert fest"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

Legt den Anzeigestring‑Wert für den booleschen Wert einer Zelle fest.

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| bv | Boolean | boolescher Wert |
| Name | String | Zeichenkettenwert des booleschen Werts |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Benutzerdefinierte boolesche Wertzeichenketten festlegen
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // Wenden Sie die Einstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;
            
            // Boolesche Werte in Zellen festlegen
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // Anzeigeformat festlegen, um boolesche Werte als Text anzuzeigen
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // Speichere die Arbeitsmappe
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


