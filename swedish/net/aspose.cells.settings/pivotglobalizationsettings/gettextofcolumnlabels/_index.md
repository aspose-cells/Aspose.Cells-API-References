---
title: "PivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar texten för etiketten Kolumnrubriker i pivottabellen"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/
---
## PivotGlobalizationSettings.GetTextOfColumnLabels method

Hämtar texten för etiketten "Column Labels" i pivottabellen.

```csharp
public virtual string GetTextOfColumnLabels()
```

### Returvärde

Texten för kolumnrubriker

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
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
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(800);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa och använd globaliseringsinställningar
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstrera GetTextOfColumnLabels
            Console.WriteLine("Column Labels Text: " + globalizationSettings.GetTextOfColumnLabels());

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


