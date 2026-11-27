---
title: "SettableGlobalizationSettings.SetTableRowTypeOfTotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger typnamnet för tabellrader som består av totalraden i den refererade tabellen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/
---
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method

Ställer in typnamnet för tabellrader som består av totalraden i den refererade tabellen.

```csharp
public void SetTableRowTypeOfTotals(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | typnamnet för tabellrader |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en tabell
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(10);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(15);
            cells["A4"].PutValue("Total");
            cells["B4"].PutValue("=SUM(B2:B3)");

            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;

            // Skapa globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Anropa SetTableRowTypeOfTotals med ett anpassat namn
                settings.SetTableRowTypeOfTotals("CustomTotals");

                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


