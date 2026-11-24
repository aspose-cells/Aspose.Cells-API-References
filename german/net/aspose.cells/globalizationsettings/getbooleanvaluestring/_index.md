---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Anzeigetextwert für den booleschen Zellwert zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

Gibt den Anzeigestringwert für den booleschen Wert einer Zelle zurück.

```csharp
public virtual string GetBooleanValueString(bool bv)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| bv | Boolean | boolescher Wert |

### Rückgabewert

Gibt standardmäßig "TRUE" für den Wahr‑Wert und "FALSE" für den Falsch‑Wert zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GetBooleanValueString mit beiden booleschen Werten demonstrieren
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // Boolesche Werte in Zellen anwenden, um die Auswirkung in der Tabelle zu zeigen
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // Benutzerdefinierte Globalisierungseinstellungen überschreiben die boolesche Zeichenkettenrepräsentation
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


