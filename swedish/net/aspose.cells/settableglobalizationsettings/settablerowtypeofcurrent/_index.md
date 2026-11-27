---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metod. Anger typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Ställer in typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
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
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Skapa globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Ange anpassat namn för den aktuella radtypen
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Verifiera inställningen genom att hämta tillbaka värdet
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Spara arbetsboken
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


