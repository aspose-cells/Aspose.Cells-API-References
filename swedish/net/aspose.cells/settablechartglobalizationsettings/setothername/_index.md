---
title: "SettableChartGlobalizationSettings.SetOtherName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Ställer in namnet på övriga etiketter för diagram"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setothername/
---
## SettableChartGlobalizationSettings.SetOtherName method

Ställer in namnet på "Other"-etiketter för Chart.

```csharp
public void SetOtherName(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | lokalt beroende namn |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till minimal data för kontext
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(150);

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ange ett anpassat namn för etiketten \"Other\"
                settings.SetOtherName("Miscellaneous Items");

                // Verifiera inställningen genom att hämta värdet
                string otherName = settings.GetOtherName();
                Console.WriteLine("Other Name set to: " + otherName);

                // Spara arbetsboken
                workbook.Save("SetOtherNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


