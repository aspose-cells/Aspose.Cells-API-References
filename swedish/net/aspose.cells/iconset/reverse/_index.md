---
title: "IconSet.Reverse"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconSet-egenskap. Hämta eller ange flaggan som indikerar om standardordningen för ikonerna i detta ikonset ska vändas. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Hämta eller ange flaggan som indikerar om standardordningen för ikonerna i denna ikonuppsättning ska vändas. Standardvärdet är falskt.

```csharp
public bool Reverse { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Ange intervallet
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Skapa villkorsformatering för ikonset
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Konfigurera ikonset
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Demonstrera Reverse-egenskapen
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Spara arbetsboken
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


