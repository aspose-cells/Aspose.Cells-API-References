---
title: "GlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är Headers så i formeln representerar Headers tabellrubriken"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/gettablerowtypeofheaders/
---
## GlobalizationSettings.GetTableRowTypeOfHeaders method

Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "#Headers" representerar tabellrubriken.

```csharp
public virtual string GetTableRowTypeOfHeaders()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfHeaders()
            {
                return "MyHeaders";
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 1.8;

            // Fixade ListObject-skapandet genom att hantera returvärdet från Add()
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            // Använd egenskapen DisplayName istället för Name
            table.DisplayName = "FruitTable";

            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A5"].Formula = "=COUNTA(FruitTable[#MyHeaders])";
                workbook.CalculateFormula();
                Console.WriteLine("Method executed successfully. Header count: " + worksheet.Cells["A5"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


