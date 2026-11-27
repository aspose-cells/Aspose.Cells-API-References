---
title: "PivotGlobalizationSettings.GetTextOfSeconds"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar den lokala texten för Seconds"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/
---
## PivotGlobalizationSettings.GetTextOfSeconds method

Hämtar den lokala texten för "Seconds"

```csharp
public virtual string GetTextOfSeconds()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSecondsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B2", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till datumfältet i radområdet
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Skapa globaliseringsinställningar
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrera GetTextOfSeconds‑metoden
            Console.WriteLine("Localized text for seconds: " + globalizationSettings.GetTextOfSeconds());

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


