---
title: "PivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar texten för etiketten Multiple Items i pivottabellen"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/
---
## PivotGlobalizationSettings.GetTextOfMultipleItems method

Hämtar texten för etiketten "(Multiple Items)" i PivotTable.

```csharp
public virtual string GetTextOfMultipleItems()
```

### Returvärde

Texten för etiketten "(Multiple Items)"

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
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
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa och använd globaliseringsinställningar
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Demonstrera GetTextOfMultipleItems och andra viktiga metoder
            Console.WriteLine("Multiple Items Text: " + settings.GetTextOfMultipleItems());
            Console.WriteLine("Total Text: " + settings.GetTextOfTotal());
            Console.WriteLine("Grand Total Text: " + settings.GetTextOfGrandTotal());

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


