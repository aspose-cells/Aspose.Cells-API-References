---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings Methode. Gibt den lokalen Text von 4 Quartalen zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

Ruft den lokalen Text von 4 Quartalen ab.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotGlobalizationSettings.GetTextOf4Quarters(). Diese Eigenschaft wird 12 Monate später ab Juli 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
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
                // Rufen Sie die Methode GetTextOf4Quaters auf
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Geben Sie die Quartalsnamen in der Konsole aus
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Fügen Sie die Quartalsnamen zum Arbeitsblatt hinzu
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // Benutzerdefinierte Implementierung von PivotGlobalizationSettings, um GetTextOf4Quaters zu überschreiben
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Geben Sie benutzerdefinierte Quartalsnamen zurück
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


