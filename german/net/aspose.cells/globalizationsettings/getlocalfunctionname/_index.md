---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Gibt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen zurück.

```csharp
public virtual string GetLocalFunctionName(string standardName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | String | Standardfunktion (en-US Gebietsschema). |

### Rückgabewert

Lokalisierungsabhängiger Funktionsname. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benutzerdefinierte Globalisierungseinstellungen festlegen
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Formel mit lokalisiertem Funktionsnamen erstellen
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


