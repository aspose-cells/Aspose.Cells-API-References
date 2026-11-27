---
title: "GlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. Standard är Totals så i formeln Totals representerar totalraden i den refererade tabellen."
type: docs
url: /sv/net/aspose.cells/globalizationsettings/gettablerowtypeoftotals/
---
## GlobalizationSettings.GetTableRowTypeOfTotals method

Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. Standard är "Totals", så i formeln "#Totals" representerar totalraden i den refererade tabellen.

```csharp
public virtual string GetTableRowTypeOfTotals()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A1"].PutValue("Item");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Book");
                worksheet.Cells["B2"].PutValue(25);
                worksheet.Cells["A3"].PutValue("Pen");
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["A4"].PutValue("Notebook");
                worksheet.Cells["B4"].PutValue(10);

                int tableIndex = worksheet.ListObjects.Add("Table1", "A1:B4", true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.ShowTotals = true;
                table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

                var settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;
                string totalRowType = settings.GetTableRowTypeOfTotals();
                
                Console.WriteLine($"Total row type: {totalRowType}");
                worksheet.Cells["C5"].PutValue($"Total row reference: #{totalRowType}");
                
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfTotals()
            {
                return "CustomTotals";
            }
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


