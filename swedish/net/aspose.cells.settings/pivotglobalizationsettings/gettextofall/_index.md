---
title: "PivotGlobalizationSettings.GetTextOfAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar texten för etiketten All i pivottabellen"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofall/
---
## PivotGlobalizationSettings.GetTextOfAll method

Hämtar texten för etiketten "(All)" i pivottabellen.

```csharp
public virtual string GetTextOfAll()
```

### Returvärde

Texten för etiketten "(All)"

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa och använd globaliseringsinställningar
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstrera GetTextOfAll-metoden
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());

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


