---
title: "IconSet.IsCustom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconSet-egenskap. Anger om ikonsetet är anpassat. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Indikerar om ikonuppsättningen är anpassad. Standardvärdet är falskt.

```csharp
public bool IsCustom { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Lägg till villkorsformatering med anpassat ikonset
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Ange intervall för villkorsformatering
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Lägg till ikonsetvillkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Ange ikonsettyp (med giltig IconSetType)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Verifiera IsCustom‑egenskapen (skrivskyddad)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


