---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger typnamnet för tabellrader som består av tabellhuvudet"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

Ställer in typnamnet för tabellrader som består av tabellhuvudet.

```csharp
public void SetTableRowTypeOfHeaders(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en tabell och lägg till lite data
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // Skapa ett ListObject (Tabell)
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Skapa en SettableGlobalizationSettings-instans
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Anropa SetTableRowTypeOfHeaders med ett anpassat rubriktypnamn
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // Applicera inställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


