---
title: "IconSet.ShowValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconSet-egenskapen. Hämta eller ange flaggan som indikerar om värdena i de celler som detta ikonset tillämpas på ska visas. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Hämta eller ange flaggan som indikerar om värdena i de celler som denna ikonuppsättning tillämpas på ska visas. Standardvärdet är sant.

```csharp
public bool ShowValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // Lägg till villkorsformatering med ikonset
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // Ställ in egenskaper för ikonsats
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // Ange området för villkorsformateringen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // Spara arbetsboken
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### Se även

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


