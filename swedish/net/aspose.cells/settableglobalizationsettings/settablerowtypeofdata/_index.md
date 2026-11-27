---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metod. Anger typnamnet för tabellrader som består av datasegmentet i den refererade tabellen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

Ställer in typnamnet för tabellrader som består av datatområdet i den refererade tabellen.

```csharp
public void SetTableRowTypeOfData(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en tabell
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // Skapa globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Ange anpassat namn för datarader i tabellen
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


