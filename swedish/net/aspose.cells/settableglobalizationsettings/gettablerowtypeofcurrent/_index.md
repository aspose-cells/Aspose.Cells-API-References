---
title: "SettableGlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metod. Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/
---
## SettableGlobalizationSettings.GetTableRowTypeOfCurrent method

Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen.

```csharp
public override string GetTableRowTypeOfCurrent()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
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
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfCurrent("CurrentRow");

            // Applicera inställningar på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Hämta den aktuella radens typnamn
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine("Current row type name: " + currentRowType);

                // Lägg till en formel som refererar till den aktuella raden
                cells["C2"].Formula = "=SUM(#CurrentRow)";
                Console.WriteLine("Formula set to: " + cells["C2"].Formula);

                // Beräkna formler
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


