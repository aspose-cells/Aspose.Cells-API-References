---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Gibt den Standardtext des integrierten Namens gemäß dem angegebenen lokalisierungsabhängigen Text zurück"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Gibt den Standardtext des integrierten Namens gemäß dem gegebenen lokalisierungsabhängigen Text zurück.

```csharp
public override string GetStandardBuiltInName(string localName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | String | Lokalisierungsabhängiger Text des integrierten Namens. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird. |

### Rückgabewert

Standardtext (en-US‑Gebietsschema).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Legen Sie einen lokalen integrierten Namen für die Demonstration fest
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Rufen Sie die Methode GetStandardBuiltInName mit einem lokalen Namen auf
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Ergebnis anzeigen
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Wenden Sie das Ergebnis auf eine Zelle an
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Zeigen Sie das berechnete Ergebnis an
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


