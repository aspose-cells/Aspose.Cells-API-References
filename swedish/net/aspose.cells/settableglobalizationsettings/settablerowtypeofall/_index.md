---
title: "SettableGlobalizationSettings.SetTableRowTypeOfAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metod. Anger typnamnet för tabellrader som består av alla rader i den refererade tabellen"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/settablerowtypeofall/
---
## SettableGlobalizationSettings.SetTableRowTypeOfAll method

Ställer in typnamnet för tabellrader som består av alla rader i den refererade tabellen.

```csharp
public void SetTableRowTypeOfAll(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för en tabell
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Skapa en tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Anropa SetTableRowTypeOfAll med anpassat namn
                settings.SetTableRowTypeOfAll("CompleteTable");

                // Applicera inställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Verifiera inställningen genom att hämta tillbaka värdet
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"Table row type for all rows set to: {rowType}");

                // Lägg till en formel som refererar till alla rader med det anpassade namnet
                cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
                Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");

                // Beräkna formler
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result: {cells["C2"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


