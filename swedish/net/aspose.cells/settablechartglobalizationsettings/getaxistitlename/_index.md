---
title: "SettableChartGlobalizationSettings.GetAxisTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings metod. Hämtar namnet på titel för axel"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getaxistitlename/
---
## SettableChartGlobalizationSettings.GetAxisTitleName method

Hämtar namnet på Title för Axis.

```csharp
public override string GetAxisTitleName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till minimal data för kontext
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Ange ett anpassat axeltitelnamn
                settings.SetAxisTitleName("Custom Axis Title");

                // Hämta axeltitelns namn med GetAxisTitleName
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Spara arbetsboken
                workbook.Save("GetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


