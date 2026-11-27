---
title: "PivotGlobalizationSettings.GetTextOfTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar texten för etiketten Totalt i pivottabellen. Du måste åsidosätta den här metoden när pivottabellen innehåller två eller fler PivotFields i dataområdet"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/
---
## PivotGlobalizationSettings.GetTextOfTotal method

Hämtar texten för etiketten "Total" i PivotTable. Du måste åsidosätta den här metoden när PivotTable innehåller två eller fler PivotFields i dataområdet.

```csharp
public virtual string GetTextOfTotal()
```

### Returvärde

Texten för etiketten "Total"

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa och använd globaliseringsinställningar
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstrera GetTextOfTotal-metoden
            Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());

            // Spara arbetsboken
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


