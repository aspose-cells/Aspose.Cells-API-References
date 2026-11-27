---
title: "FormatCondition.IconSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition property. Hämta den villkorliga formateringens IconSet-instans. Standardinstansens IconSetType är TrafficLights31. Giltig endast för typen IconSet"
type: docs
url: /sv/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Hämta den villkorliga formateringens "IconSet"-instans. Standardinstansens IconSetType är TrafficLights31. Giltig endast för typ = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Lägg till villkorsstyrd formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Ange cellintervallet
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Lägg till villkor och sätt typ till IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Hämta IconSet och konfigurera den
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Spara arbetsboken
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Se även

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


