---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar visningsnamnet för data-pivotfältet. Standardformatet är Sum Of Field"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Hämtar visningsnamnet för datapivottfältet. Standardformatet är "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| funktion | ConsolidationFunction | Funktionen används för att summera värden i pivotfältet. |
| namn | String | Det ursprungliga namnet på pivotfältet. |

### Exempel

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
                // Skapa en instans av PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definiera parametrar för metoden GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Anropa metoden GetNameOfDataField
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Skriv ut resultatet
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

### Se även

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


