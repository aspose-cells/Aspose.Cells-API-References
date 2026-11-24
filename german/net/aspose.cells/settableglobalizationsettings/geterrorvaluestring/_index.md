---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den Anzeigestringwert für den Fehlwert einer Zelle zurück."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Gibt den Anzeigestringwert für den Fehlerwert einer Zelle zurück.

```csharp
public override string GetErrorValueString(string err)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| err | String | Fehlerwerte wie #VALUE!, #NAME? |

### Rückgabewert

Gibt standardmäßig den Fehlwert selbst zurück

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Erstelle eine Zelle mit Fehlwert
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // Rufe GetErrorValueString mit dem Fehlwert-String auf
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Ergebnis anzeigen
                Console.WriteLine("Error value string: " + errorString);

                // Zeige den Effekt, indem du den Wert einer anderen Zelle auf den zurückgegebenen String setzt
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


