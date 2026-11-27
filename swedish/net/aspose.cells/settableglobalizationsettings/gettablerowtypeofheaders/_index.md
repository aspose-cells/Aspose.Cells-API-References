---
title: "SettableGlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings metod. Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är Headers, så i formeln representerar Headers tabellrubriken."
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/
---
## SettableGlobalizationSettings.GetTableRowTypeOfHeaders method

Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "#Headers" representerar tabellrubriken.

```csharp
public override string GetTableRowTypeOfHeaders()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfHeaders("CustomHeaders");
            workbook.Settings.GlobalizationSettings = settings;

            // Skapa exempeldata för tabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            try
            {
                // Hämta tabellradens typ för rubriker
                string rowType = settings.GetTableRowTypeOfHeaders();
                Console.WriteLine($"Table row type for headers: {rowType}");

                // Skapa ett ListObject (Tabell)
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

                // Använd den anpassade headerreferensen i en formel
                worksheet.Cells["C2"].Formula = "=COUNTA(Table1[#CustomHeaders])";
                Console.WriteLine("Formula using custom headers reference: " + worksheet.Cells["C2"].Formula);

                // Beräkna formeln
                workbook.CalculateFormula();
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

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


