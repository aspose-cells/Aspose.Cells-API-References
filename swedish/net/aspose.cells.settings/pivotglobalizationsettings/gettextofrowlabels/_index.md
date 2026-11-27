---
title: "PivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar texten för etiketten Row Labels i pivottabellen"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/
---
## PivotGlobalizationSettings.GetTextOfRowLabels method

Hämtar texten för etiketten "Row Labels" i PivotTable.

```csharp
public virtual string GetTextOfRowLabels()
```

### Returvärde

Texten för radetiketter

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa och använd globaliseringsinställningar
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Demonstrera GetTextOfRowLabels
            Console.WriteLine("Row Labels Text: " + settings.GetTextOfRowLabels());

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


