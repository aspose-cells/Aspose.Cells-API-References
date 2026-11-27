---
title: "IconSet.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconSet-egenskap. Hämta eller ange ikonsettypen som ska visas. När typen anges kontrolleras automatiskt om det aktuella Cfvoss‑antalet stämmer överens med den nya typen. Om det inte stämmer tas gamla Cfvos bort och standard‑Cfvos läggs till"
type: docs
url: /sv/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Hämta eller ange ikonutgångstypen som ska visas. Att ange typen kommer automatiskt att kontrollera om det aktuella antalet Cfods stämmer överens med den nya typen. Om det inte stämmer, kommer gamla Cfods att rensas och standard‑Cfods att läggas till.

```csharp
public IconSetType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Demonstrera användning av Type-egenskapen
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


