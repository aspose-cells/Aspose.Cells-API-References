---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Hämtar namnet på \\\"Other\\\"‑etiketter för Chart"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Hämtar namnet på "Other"-etiketter för Chart.

```csharp
public override string GetOtherName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till minimal data (valfritt, bara för en komplett arbetsbok)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Instansiera objektet för globaliseringsinställningar
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ange ett anpassat namn för etiketten \"Other\"
                settings.SetOtherName("Custom Other Label");

                // Hämta namnet med GetOtherName
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Spara arbetsboken (inställningarna är inte direkt kopplade till chart i den här demonstrationen)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


