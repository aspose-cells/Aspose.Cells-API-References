---
title: "PivotGlobalizationSettings.GetShortTextOf12Months"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt alle kurz formatierten Zeichenketten von 12 Monaten zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/
---
## PivotGlobalizationSettings.GetShortTextOf12Months method

Liest alle kurz formatierten Zeichenfolgen der 12 Monate.

```csharp
public virtual string[] GetShortTextOf12Months()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetShortTextOf12MonthsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine benutzerdefinierte Globalisierungs‑Einstellungen‑Klasse, die von PivotGlobalizationSettings erbt
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Rufe die Methode GetShortTextOf12Months auf
                string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();

                // Gib die Monatsnamen in der Konsole aus
                Console.WriteLine("Short names of 12 months:");
                foreach (string monthName in monthShortNames)
                {
                    Console.WriteLine(monthName);
                }

                // Füge die Monatsnamen zum Arbeitsblatt hinzu
                for (int i = 0; i < monthShortNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(monthShortNames[i]);
                }

                Console.WriteLine("Method executed successfully. Month names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetShortTextOf12Months method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
        }
    }

    // Benutzerdefinierte Implementierung von PivotGlobalizationSettings, um GetShortTextOf12Months zu überschreiben
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetShortTextOf12Months()
        {
            // Gibt benutzerdefinierte kurze Monatsnamen zurück
            return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
                                "Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


