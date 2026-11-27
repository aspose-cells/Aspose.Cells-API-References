---
title: "PivotGlobalizationSettings.GetTextOfDays"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar den lokala texten för dagar"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdays/
---
## PivotGlobalizationSettings.GetTextOfDays method

Hämtar den lokala texten för "Days".

```csharp
public virtual string GetTextOfDays()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDaysDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(1500);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till datumfältet i radområdet
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Skapa globaliseringsinställningar
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrera metoden GetTextOfDays
            Console.WriteLine("Localized text for days: " + globalizationSettings.GetTextOfDays());

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


