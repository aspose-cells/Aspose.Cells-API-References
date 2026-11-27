---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. Standard är This Row så i formeln This Row representerar den aktuella raden i den refererade tabellen."
type: docs
url: /sv/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. Standard är "This Row", så i formeln "#This Row" representerar den aktuella raden i den refererade tabellen.

```csharp
public virtual string GetTableRowTypeOfCurrent()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Skapa exempeldata och tabell
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // Skapa tabell
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // Lägg till formel med referens till aktuell rad
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // Demonstrera effekten av GetTableRowTypeOfCurrent
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


