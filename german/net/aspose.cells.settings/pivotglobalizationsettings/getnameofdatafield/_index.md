---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt den Anzeigenamen des Daten-Pivotfelds zurück. Das Standardformat ist Sum Of Field"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Liest den Anzeigenamen des Daten‑Pivot‑Feldes. Das Standardformat ist "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Funktion | ConsolidationFunction | Die Funktion wird verwendet, um Werte des Pivotfelds zusammenzufassen. |
| Name | String | Der ursprüngliche Name des Pivotfelds. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Instanz von PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definiere Parameter für die Methode GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Rufe die Methode GetNameOfDataField auf
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Gib das Ergebnis aus
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


