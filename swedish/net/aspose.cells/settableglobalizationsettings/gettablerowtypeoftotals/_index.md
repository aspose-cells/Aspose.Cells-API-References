---
title: "SettableGlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metod. Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/
---
## SettableGlobalizationSettings.GetTableRowTypeOfTotals method

Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen.

```csharp
public override string GetTableRowTypeOfTotals()
```

### Returvärde

typnamnet för tabellrader

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för tabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");

            // Skapa ett ListObject (Tabell)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfTotals("CustomTotals");

            try
            {
                // Hämta tabellradstypen för totaler
                string rowType = settings.GetTableRowTypeOfTotals();
                Console.WriteLine($"Table row type for totals: {rowType}");

                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Verifiera effekten i en formel
                worksheet.Cells["C2"].Formula = "=SUM(#CustomTotals[B])";
                Console.WriteLine("Formula using custom totals reference: " + worksheet.Cells["C2"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


